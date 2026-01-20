# Exercise 1: Microsoft Foundry Fundamentals

### Estimated Duration: 20 Minutes

## Overview

In this exercise, you will gain hands-on experience setting up **Microsoft Foundry** and deploying the GPT-4o model. You will create an Azure AI Search resource to enable document retrieval capabilities and configure a Microsoft Foundry AI Hub to deploy the GPT-4o model. Finally, you will test the deployed model's capabilities in the Foundry Playground.

## Objectives

In this exercise, you will complete the following tasks:

- Task 1: Set up Microsoft Foundry

## Task 1: Set up Microsoft Foundry

In this task, you will explore different flow types in Microsoft Foundry by creating a AI hub through Azure portal, then deploying the GPT-4o model, and testing its capabilities in the playground from the Microsoft Foundry.

1. On the **Azure portal**, search for **Microsoft Foundry (1)** and select **Microsoft Foundry (2)** from the results.

    ![](./media/new/a1.png)

1. From the left navigation pane, expand **Use with Foundry**, select **Foundry (1)**, open the **Create (2)**.

    ![](./media/createfound.png)

1. On the **Azure AI hub** page, provide the following details and then click on **Review+create (6)**:

    - **Subscription**: Leave the default one **(1)**

    - **Resource group:** Select **ai-foundry-<inject key="Deployment ID" enableCopy="false"></inject> (2)**

    - **Name:** Select **ai-foundry-<inject key="Deployment ID" enableCopy="false"></inject> (3)**
        >**Note:** Ensure to select the same region used while creating the Azure AI Search resource.

    - **Region:** Enter **<inject key="Region" enableCopy="false"></inject> (4)**

    - **Default project name:** Enter **ai-foundry-project-<inject key="Deployment ID" enableCopy="false"></inject>**

      ![](./media/foundryr.png)

1. Once the Validation passed, click on **Create**.

    ![](./media/createfoundry.png)

1. Once the deployment is completed, click on **Go to resource**.

    ![](./media/gotofoundry.png)

1. From the **Overview** page of the **Microsoft Foundry**, click **Go to Foundry Portal** to open the Foundry workspace.

    ![](./media/gotoportal.png)

1. On the Welcome page click on **Build** from the top navigation pane.s

    ![](./media/new/foundryoverview.png)

1. From the left navigation pane, select **Models(1)**, then click on **Deploy base model (2)**.

    ![](./media/new/basemodel.png)

1. Search for **gpt-4o (1)**, select the **gpt-4o (2s)** model.

    ![](./media/new/4o.png)

1. Select the **Deploy (1)** drop-down and select **Custom settings (2)**.

    ![](./media/new/custom.png)

1. On the **Deploy gpt-4o** blade, click on **Customize** and configure the required deployment settings as specified below:

    - **Deployment name:** Keep deafult **gpt-40 (1)**

    - **Deployment type**: Choose **Standard (2)** 
    
    - **Model version**: Select **2024-08-06 (3)**

    - **Tokens per Minute Rate Limit**: Limit to **50K (4)** (You can use keyboard arrows to increase or decrease the value)

    - Click on **Deploy (5)**

      ![](./media/new/4oconfig.png) 

1. From the top, click on **Microsoft Foundry**.

    ![](./media/new/b2.png) 

1. Select the listed **aifoundryhubxxxxxx** resource to continue working in **Microsoft Foundry**.

    ![](./media/new/b3.png)

     >**Note**: **xxxxx** refers to randomly generated suffix.

1. From left navigation pane, select **Model + endpoints (1)** from the **My assets** section, then select **gpt-4o (2)** model and the click on **Open in Playground (3)**.

    ![](./media/new/b4.png)

1. In the Setup section, replace the existing text with `Extract the United States Postal Service (USPS) formatted address from the following email` **(1)** then click on **Apply changes (2)**. Using this you can explore the capabilities of Azure OpenAI.

    ![](./media/new/b5.png)

1. Click **Continue** to update the system message and start a new chat session.

    ![](./media/new/b6.png)

1. Provide the below mail in the chat **(1)** then click on **Send (2)** to identify and extract the postal address from the following email:

    ```
    Subject: Elevate Your Brand with Our Comprehensive Marketing Solutions!
    From: BrightEdge Marketing
    To: John Doe

    Dear John,
    At BrightEdge Marketing, we believe in the power of innovative marketing strategies to elevate brands and drive business success. Our team of experts is dedicated to helping you achieve your marketing goals through a comprehensive suite of services tailored to your unique needs.

    Please send letters to 123 Marketing Lane, Suite 400, in area 90210, Innovation City, California.

    Thank you for considering BrightEdge Marketing.
    Best regards,
    Sarah Thompson
    Marketing Director BrightEdge Marketing
    ```

    ![](./media/new/b7.png)
    
1. You will receive a response similar to the one shown below:

    ![](./media/new/b8.png)

  > **Congratulations** on completing the lab! Now, it's time to validate it. Here are the steps:
  > - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next  task. 
  > - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
  > - If you need any assistance, please contact us at cloudlabs-support@spektrasystems.com. We are available 24/7 to help
 
<validation step="a3e77878-3ce2-4d69-b4e6-c88d4a0f45ec" />

## Summary

In this exercise, you have completed the following:

- Set up Microsoft Foundry.

- Created Azure AI Search.

### You have successfully completed this exercise. Kindly click **Next >>** to proceed further

![Launch Azure Portal](./media/gsk5.png)
