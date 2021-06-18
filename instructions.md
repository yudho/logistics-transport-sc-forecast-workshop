# Amazon Forecast No-code-workshop
*No code workshop to experiment on Amazon Forecast*

Introduction: Amazon Forecast is a machine learning service that provides prediction based on time series data provided by AWS.

## Section A: Data Preparation
### A.1 Region selection
Please check with your instructor about the regions where you will be working for this hands-on. You can change it by selecting the region name in the upper right of the screen:

![Region selection](pictures/region_selection.png "Region selection")

### A.2 Go to SageMaker
We will use SageMaker Studio for data preparation. Type "sagemaker" on the search bar on top and click "Amazon SageMaker"
![Go to SageMaker](assets/pictures/enter-sagemaker-in-console.png "Go to SageMaker")

### A.3 Enter studio
On SageMaker console, locate and click "Amazon SageMaker Studio" on the left menu. There should be a user already created on the right pane. Click "Open studio". It may take a while for the studio to open, probably around 2-5 minutes.
![Enter studio](assets/pictures/enter-sagemaker-studio.png "Enter studio")

### A.4 Download the Notebooks
Once the studio is open, locate the left menu and click the second icon from top for Git. 

![Clone repo](assets/pictures/clone-repo.png "Clone repo")

Then click "Clone a Repository". When asked for the git URL, paste https://github.com/yudho/logistics-transport-sc-forecast-workshop.git and click "CLONE"

It should clone the notebooks and open up the folder structure. Please click the folder "logistics-transport-sc-forecast-workshop".

### A.5 Open First Notebook
Amazon Forecast requires 1 main dataset, which is the target time series. In this case, we will use the Jupyter Notebook to download a public dataset on NYC taxi pickups, transform as necessary to form the target time series CSV file, and upload it to S3 to be used with Forecast.

Please double click file "01_prepare-target-time-series.ipynb". Once open, on the top right, ensure that the Kernel active is Python 3 (Data Science) with EC2 size of 2 vCPU + 4 GiB RAM. You can change them if they display other value. **Important**: Kernel can take minutes to be ready, especially if this is the first time you open the studio. If you see the instance type is "Unknown", you can just wait first until the kernel is ready 

![Studio kernel](assets/pictures/studio-kernel.png "Studio kernel")

### A.6 Generate Target Time Series as Input Data
After the kernel is ready, click "Run" menu on the top bar and click "Run All Cells". Along with instructor, you can dive deeper on the dataset used, the transformation done, and the resulted CSV file structure in the notebook.




