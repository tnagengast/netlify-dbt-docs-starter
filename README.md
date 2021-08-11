Welcome to your new dbt project!

### Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](http://slack.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices


### Deploying to Netlify
1. Create a dbt project
1. Push you dbt project to a GitHub repo
1. Create a Netlify account
1. Create a `New site from Git`
	1. Select the GitHub option to authorize
	1. Select the repo you made for your dbt project
	1. Set the `Build command` and `Publish directory`
	1. Finish by select `Deploy site` (this will fail, now we fix it!)
1. Add `reqirements.txt` with your dbt version
1. Add `profiles/profiles.yml`
1. Back in Netlify, add your environment variables for you `profiles.yml`


