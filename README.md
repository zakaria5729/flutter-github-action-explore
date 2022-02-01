# Flutter Github Action (CI/CD) Explore

- Create /.github/workflows/ folders in your flutter github project root path
- Create main.yml and [paste the code](https://github.com/zakaria5729/flutter-github-action-explore/blob/main/.github/workflows/main.yml)
- Create staging.yml and [paste the code](https://github.com/zakaria5729/flutter-github-action-explore/blob/main/.github/workflows/staging.yml)
- Create two branch - staging and development
- Add project secret token from app /settings/secrets/actions/new repository secret

# Project development machanism:
- We are always working on **Development** branch and after completed a module, we will merge the code from **Development to Staging branch** with the staging server base url (staging branch's github action will generate android debug build apk with dev-1.0.x versin number).

- After test we change our server endpoint staging to production and merge the code from **Staging to Main branch** (main branch's github action will generate android release build apk and aab with prod-1.0.x versin number). You can see the dev and prod (demo) builds from [here](https://github.com/zakaria5729/flutter-github-action-explore/releases) and also you can see the demo github actions from [here](https://github.com/zakaria5729/flutter-github-action-explore/actions)
