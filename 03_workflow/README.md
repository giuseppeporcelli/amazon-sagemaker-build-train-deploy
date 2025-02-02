# Module 3: Create a complete deployment pipeline

1. In the Explorer window, from folder **03_workflow**, open the Python file **pipeline.py**.

    <img src="../images/module_03/open_pipeline_script.png" alt="Open pipeline script" width="800px" />

2. Make yourself familiar with the code in **pipeline.py**. The script performs the following steps:
   - Download the raw dataset and upload to a location in Amazon S3
   - Create an Amazon SageMaker Pipeline to orchestrate the execution of the ML workflow steps, including data processing, training, evaluation, register model version in the SageMaker Model Registry and finally deploy the latest model version.
   - Execute the pipeline
  
    The definition of the SageMaker Pipeline is built using the @step decorator, a feature of SageMaker Pipelines that converts your local machine learning functions into one or more pipelines. This allows to orchestrate the same functions that we built for data processing, training and deployment as part of a pipeline. For further information, please read: https://docs.aws.amazon.com/sagemaker/latest/dg/pipelines-step-decorator.html


3. Choose the **Run Python File** icon at the top right, as displayed below:

    <img src="../images/module_03/run_pipeline_script.png" alt="Open pipeline script" width="800px" />

4. The Terminal window will show the progress of the execution. The last operation in the pipeline script will start the pipeline, and pipeline execution will continue in the background.

5. Go back to SageMaker Studio and choose **Pipelines** from the menu on the left.

6. Choose the pipeline named **sagemaker-btd-pipeline** to display a list of executions for the pipeline.

    <img src="../images/module_03/pipelines.png" alt="Open pipeline script" width="800px" />

7. Choose the last pipeline execution from the list.

    <img src="../images/module_03/pipeline_executions.png" alt="Open pipeline script" width="800px" />

8. The pipeline execution page includes a visual representation of the status. Wait until the pipeline execution is completed.

    <img src="../images/module_03/pipeline-execution-in-progress.png" alt="Open pipeline script" width="800px" />

    <img src="../images/module_03/pipeline-execution-completed.png" alt="Open pipeline script" width="800px" />

9.  In SageMaker Studio, choose **Deployment >> Endpoints** from the menu on the left. Locate the endpoints whose name starts with `sagemaker-btd-endpoint-`. Find the last deployed endpoint (note the **Created on** field), and make note of the endpoint name. You will need to use this name in the next module.

	<img src="../images/module_02/view_endpoints.png" alt="List of endpoints" width="800px" />

## Proceed to Module 4
You have completed Module 3: Create a complete deployment pipeline. Please proceed to [Module 4: Build a HTTP API using Amazon API Gateway and AWS Lambda](../04_api_gateway_and_lambda/README.md).