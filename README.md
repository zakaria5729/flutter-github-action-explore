# Flutter Github Action (CI/CD) Explore

- Create /.github/workflows/ folders in your flutter github project root path
- Create main.yml and [paste the code](https://github.com/zakaria5729/flutter-github-action-explore/blob/main/.github/workflows/main.yml)
- Create staging.yml and [paste the code](https://github.com/zakaria5729/flutter-github-action-explore/blob/main/.github/workflows/staging.yml)
- Create two branch - staging and development
- Add project secret token from app /settings/actions/new repository secret

Project development machanism:
- We are alwayas working on development branch and after completed a module we merge the code from development to staging branch with the staging server endpoint (staging branch's github action will generate android debug build apk with dev-1.0.x versin number). After test we change our server endpoint staging to production and merge the code from staging to main (main branch's github action will generate android release build apk and aab with prod-1.0.x versin number).
