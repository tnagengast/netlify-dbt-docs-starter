# Deploying to Netlify

## dbt Setup
1. Create a dbt project
1. Push your dbt project to a GitHub repo
1. Add [`reqirements.txt`](https://github.com/tnagengast/netlify-dbt-docs-starter/pull/1/files#diff-4d7c51b1efe9043e44439a949dfd92e5827321b34082903477fd04876edb7552) with your dbt version
1. Add [`profiles/profiles.yml`](https://github.com/tnagengast/netlify-dbt-docs-starter/pull/1/files#diff-0b6234791dc6ccbcc7864adcd31fe50d322290fd76217b6673fb4b8f7ccf8337)
1. Add [`netlify.toml`](https://github.com/tnagengast/netlify-dbt-docs-starter/pull/1/files#diff-ab8f79b68b7adff7a07db953bf453f3c5aa6ade98d2b1b67d8432b36392489ed) file that Netlify will use to build the docs

## Netlify Setup
1. Create a Netlify account
1. Setup your docs site
    1. Create a `New site from Git`
    ![CleanShot 2021-08-11 at 09 07 42](https://user-images.githubusercontent.com/260337/129073463-da874729-584d-4732-98fa-7c83658a69e6.png)
    1. Select the `GitHub` option to authorize
    ![CleanShot 2021-08-11 at 09 08 02](https://user-images.githubusercontent.com/260337/129074263-34d5fc04-aa34-410d-a7ed-646dca5e8391.png)
    1. Select the repo you made for your dbt project
    ![CleanShot 2021-08-11 at 10 20 11](https://user-images.githubusercontent.com/260337/129074668-fa6d6b21-a908-4446-a471-e30316969616.png)
    1. Finish setup by selecting `Deploy site` (this will deploy, but we're not quite finished yet)
    ![CleanShot 2021-08-11 at 09 13 09](https://user-images.githubusercontent.com/260337/129074721-895dbf76-3f30-47f1-a24e-c7f610cb126c.png)
1. Add your environment variables for your `profiles.yml` and hit `Save`
![CleanShot 2021-08-11 at 09 48 03](https://user-images.githubusercontent.com/260337/129074981-e05b79ef-9f7c-4007-831d-49d567f4c8e5.png)
1. Now you can deploy your docs by going to the `Deploys` section and hitting `Trigger deploy` -> `Deploy site`
![CleanShot 2021-08-11 at 09 51 57](https://user-images.githubusercontent.com/260337/129074231-b62296f4-2ed8-4e28-bf8e-eb31485ffe25.png)


## Connect CLI
1. Download the Netlify CLI
1. Run `netlify link` to link you local development to your site


## Adding authentication
1. Add `docs/functions/auth.js`
1. Add `package.json` and install with `npm install`
