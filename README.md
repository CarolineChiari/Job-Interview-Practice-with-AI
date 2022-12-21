## What you need to get started

This notebook needs a `.env` file in the same folder with the following data:
```
SPEECH_KEY=<Cognitive services key>
SPEECH_REGION=<cognitive service region>
SPEECH_LANGUAGE=<cognitive services language>
OPENAI_KEY=<openAI API key>
```

## How do I get the speech key and region?

You need a valid [Azure](https://portal.azure.com/) subscription in order to get those keys.

Once you do, follow these steps:
- (optional) Create a new Azure Resource Group and call it `speech`
- From the resource group, click on **Create** and search for `Cognitive  Services`
- Select the first one anc click **Create**
- Choose your subscription and resource group. Also provide a name and choose the pricing tier. You can find more information about Cognitive services' pricing [here](https://azure.microsoft.com/en-us/pricing/details/cognitive-services/speech-services/)
- Leave everything else as default and click **Review + Create** then click **Create** if there are no issues.
- Once the service is created, either click on **Go to Resource** or navigate to your resource
- Click on **Keys and Endpoint** on the left pane
- From there you can copy your key and region, and paste it in the `.env` file mentioned above.

## How do I get the OpenAI Key?

You need a valid paid subscription to OpenAI. More information about costs [here](https://openai.com/api/pricing/)

- Go to [OpenAI's API website](https://openai.com/api/)
- **Log In** or **Sign Up** if you haven't done so already
- Click on your profile in the right hand side of the screen
- Click on **View API Keys**
- Click on **Create New Secret Key**
- Copy and paste the value in the `.env` file mentioned above.

## How to use this notebook?

In the code box below, replace the `jobTitle` with the job title you want to practice with.
Enter the `numberOfQuestions` you want to practice on.

Run all the cells.

When the AI asks you a question, there will be a shot tone to indicate that it's ready to listen to you. If you stop talking for 2.5s, it will automatically assume you are done answering and move to the next question.