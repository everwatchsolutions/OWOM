# One World of Minerals project from USGS
**1. Sign up for a Bluemix free trial account if needed.**

>1. Go to bluemix.net and click Create a free account 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.44.44.png)
>2. Fill out the registration form and click the Create Account button.
>3. You'll receive a verification e-mail which contains a link to activate your account.

**2. Login to Bluemix**

>1. Go to bluemix.net and click the Log in button 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.44.59.png)
>2. Provide your username and click the Continue button 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.46.16.png)
>3. Provide your password and click the Log in button 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.46.42.png)
    
**3. Create an IBM Data Connect Instance**

>1. Once logged into Bluemix, go to the Bluemix Catalog by clicking the Catalog button in the upper right  corner or going to bluemix.net/catalog 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.48.55.png)
>2. In the catalog, type Data Connect into the search bar and click on the Data Connect service description. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.49.31.png)
>3. Ensure that the Data Connect pricing plan is set to Starter and click the Create button.  
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.50.55.png)
>4. On the service description page for your new Data Connect instance, click the Manage tab then click on the Launch button to launch the Data Connect dashboard.
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.54.41.png)

**4. Replicate data normalization work in IBM Data Connect**

>1. In the Data Connect dashboard, click on File Storage in the menu on the left side of the screen.
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2019.59.58.png)
>2. Upload the OneWorld Working Dataset file by clicking on the icon at the bottom of the screen then select your file from the explorer window and clicking Open. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.00.47.png)
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.02.23.png)
>3. Once your data file is uploaded, click on Refine & Copy 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.02.56.png)
>4. In the Refine & Copy screen, click on Files 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.03.21.png)
>5. In Files, click on the file you just uploaded 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.05.44.png)
>6. In Worksheets, check the box next to all worksheets you want to refine. As you select worksheets to refine, they will appear in the Selected column on the right side of the screen. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.05.00.png)
>7. Click the triple dots to right of your worksheet in the Selected column then click on the Configure button to perform an initial shaping of your data. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.06.20.png)
>8. The Configure window provides a preview of the data, and we notice that data starts at row 3 with data headings at row 2. To remedy this, we will click on Configure. Note: Data Connect automatically creates a unique ID for each data row.
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.07.54.png)
>9. Click OK in the resulting dialog. We haven't made any column changes yet so nothing will be lost.
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.09.14.png)
>10. In the next dialog, specify that data starts at row 2 by clicking on row 2, check Selected line is the header, then click Apply.
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.12.39.png)
>11. In the next dialog, review that your data headers are correct then click Done.  
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.16.50.png)
>12. Click the Refine Data button in the upper right corner.  
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.18.08.png)
>13. In the Refine Data view, click Organize then click Change Schema
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.20.26.png)
>14. Remove the columns named COLUMN2, COLUMN5, and COLUMN11 by mousing over the column name and clicking on the trash can icon.                       
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.25.29.png)
>15. When you are done removing all 3 columns, click on Apply.                            
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.26.33.png)
>16. Begin editing the name for your activity by mousing over the activity name at the top of the screen (will probably say Untitled) and clicking on the pencil icon to the right. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.30.17.png)
>17. Provide a new name for the activity then click the checkmark button. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.32.25.png)
>18. Click the Next button in the upper right corner of the screen. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.33.04.png)
>19. In the next screen, click Files on the left side of the screen. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.33.57.png)
>20. Select JSON as the type of file to create. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.34.58.png)
>21. Click the Run button in the upper right corner of the screen. 
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.36.59.png)
>22. In the resulting screen, you will see your activity running.                       
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.38.07.png)
>23. When the word Running... disappears from your activity, the activity has completed.                           
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.38.48.png)
>24. Click on File Storage in the menu on the left side of the screen.
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2019.59.58.png)
>25. Your new JSON file should be listed in File Storage. Download it by mousing over the file name and clicking on the download icon.  This is the file you will load into Elasticsearch.
![alt tag](/images/Box%20Notes%20Image%202017-03-28%2020.41.39.png)

**5. Create Elasticsearch Instance on Bluemix**

1.  From your IBM Bluemix Dashboard, scroll down until you see a blue button labeled "Create Service" towards the right side of the page and click it.

2.  From the catalog page, you will have two options for creating your Elasticsearch service.  You can either go to the "Container" section and upload your own Docker image, or you can go to the "Data & Analytics" section and choose "Compose for Elasticsearch".

3.  From this creation page, you can "Connect To" your other IBM Bluemix Applications.  Once you've chosen a Service and Credential name, click the "Create Button" in the lower right corner.

**6. Stand up Kibana instance pointing to Elasticsearch**

Kibana is an open source plugin for Elasticsearch that will allow us to visual our data.  Note that at the current time, Kibana is not a default service available on Bluemix, so we will have to upload our own docker image for this application.

1.  From the dashboard, click the "Create App" button.
2.  Next click on "Containers" and choose "Upload an Image".
3.  You'll need to follow the steps shown to push your docker image to Bluemix.
If you don't have a docker image for Kibana, you can find one here: https://hub.docker.com/_/kibana/
Note:  You may need to configure your Kibana image's environment variables to point towards your Elasticsearch instance.  Information about editing docker files can be found here: https://docs.docker.com/engine/reference/builder/

**7. Create an index in Elasticsearch**

In our case, Elasticsearch will be automatically indexing our data for us on upload based on the "index name" we choose in our CURL request to post the data.

For advanced users who want to know more about creating their own indexes, please refer to the elastic documentation here: https://www.elastic.co/guide/en/elasticsearch/reference/current/indices-create-index.html

**8. Format json data & load into Elasticsearch**

To format our data correctly, we can use a library called JQ, downloaded from here: https://stedolan.github.io/jq/

The from the directory where you have jq and your OneWorld_Working_Dataset_Sample.json, run:

./jq --slurp '{("minerals"): .[]}' OneWorld_Working_Dataset_Sample.json > OneWorld_Working_Dataset_Sample_Formatted.json

Optionally, if you needed to add a field, you could run this command (here we are adding a timestamp value to each entry):

./jq --slurp '{("minerals"): [.[] | .[] | .[] * {TIMESTAMP: "1489854901"}]}' OneWorld_Working_Dataset_Sample.json > OneWorld_Working_Dataset_Sample_Formatted.json

Loading into Elasticsearch:  One easy method to load a json file into Elasticsearch is to POST the file via curl.
For example, for uploading a json file in your current directory, use the command:

curl -u username:password -XPOST 'https://url_for_elastic_search:port/index_name' -d @OneWorld_Working_Dataset_Sample_Formatted.json --insecure

The --insecure command is only needed when running services with self-signed CA certificates.


**9. Create a basic visualization in Kibana**

1.  Access the kibana dashboard by going to the public IP and port you assigned for it when creating the container.  Example xxx.xx.xx.xxx:5601/app/kibana
2.  Click "Visualize" on the top menu bar.  We'll start with a simple bar chart for now, so choose "Vertical Bar Chart".
3.  Select "From a New Search" for now.  This will let us customize the search query used for data.
4.  Notice the top search bar has a "*" in it.  Leave that for now, since that will run our visualization across all the data in Elasticsearch.  If you needed to refine the output with a specific query, you could do it there.
5.  On the left menu, choose "Data".  From here we can start designing our chart.  For the Y-Axis, we can choose "Count" for Aggregation.
6.  For the X-Axis, we can choose "Filters" for Aggregation.  Now, we can add as many Filters as we would like.  For now lets make two of them, one with COMMODITY: Salt and the other with COMMODITY: Copper.
7.  Further down on the left side menu, we can add a "Sub-Bucket" and choose "Split Bars".
8.  Choose "Terms" for the Sub Aggregation, "COUNTRY" for the Field, "metric: Percentage of Count" for Order By.  "Descending" for Order, and "7" for Size.
9.  Click the green play button towards the top of the left side menu and your metric should now be visualized, showing percentage of Salt and Copper by Country.  Your visualization setup should look similar to the settings shown on the left hand menu below.
10.  For more information about other visualizations in Kibana, please refer to their documentation here: https://www.elastic.co/guide/en/kibana/current/tutorial-visualizing.html
