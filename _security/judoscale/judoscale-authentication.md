---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Judoscale as documented on the provider pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Judoscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Judoscale declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Judoscale
provider_slug: judoscale
scheme_count: 3
schemes:
- evidence: Jud​oscale integrates with Heroku via OAuth , which grants access to all of your teams and apps (sadly), but after granting access you’ll come back to Judoscale and choose which team(s) and app(s) to link for autoscaling.
  how_to_obtain: Click “Authenticate with Heroku” which redirects to Heroku’s authorization screen where you authorize Judoscale to access your account.
  name: Heroku OAuth
  type: oauth2
- evidence: Jud​oscale needs your Organization Token in order to fetch apps and machines information, and create/destroy machines when autoscaling.
  how_to_obtain: Generate a new token in the Fly dashboard under “Tokens”, name it “Judoscale”, and paste it into Judoscale’s Connect to Fly form.
  name: Fly Organization Token
  type: apiKey
- evidence: Jud​oscale needs your Team Token in order to fetch project environments and services information, and update the number of running replicas.
  how_to_obtain: Create a new Team token in Railway account settings, name it “Judoscale”, and paste it into Judoscale’s Connect to Railway form.
  name: Railway Team Token
  type: apiKey
slug: judoscale-authentication
source_filename: judoscale-authentication.yml
source_heading: Authentication Profile
source_url: https://judoscale.com/docs/heroku-getting-started
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://judoscale.com/docs/heroku-getting-started\nsources:\n- https://judoscale.com/docs/heroku-getting-started\n- https://judoscale.com/docs/aws-getting-started\n- https://judoscale.com/docs/fly-getting-started\n- https://judoscale.com/docs/railway-getting-started\ndescription: Authentication methods for Judoscale as documented on the provider pages.\nschemes:\n- type: oauth2\n  name: Heroku OAuth\n  evidence: Jud​oscale integrates with Heroku via OAuth , which grants access to all of your teams and apps (sadly), but after granting access\n    you’ll come back to Judoscale and choose which team(s) and app(s) to link for autoscaling.\n  how_to_obtain: Click “Authenticate with Heroku” which redirects to Heroku’s authorization screen where you authorize Judoscale to access your\n    account.\n- type: apiKey\n  name: Fly Organization Token\n  evidence: Jud​oscale needs your Organization\
  \ Token in order to fetch apps and machines information, and create/destroy machines when autoscaling.\n  how_to_obtain: Generate a new token in the Fly dashboard under “Tokens”, name it “Judoscale”, and paste it into Judoscale’s Connect to Fly form.\n- type: apiKey\n  name: Railway Team Token\n  evidence: Jud​oscale needs your Team Token in order to fetch project environments and services information, and update the number of running\n    replicas.\n  how_to_obtain: Create a new Team token in Railway account settings, name it “Judoscale”, and paste it into Judoscale’s Connect to Railway form.\ndocs: https://judoscale.com/docs/heroku-getting-started\n"
source_yaml_url: https://artifacts.apis.io/judoscale/authentication/judoscale-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Autoscaling
- Cloud
- DevOps
- Heroku
---
