---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an account key passed as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EKM Metering Inc. Authentication
name_suffix: Authentication
oauth_flows: []
overview: EKM Metering Inc. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EKM Metering Inc.
provider_slug: ekm-metering
scheme_count: 1
schemes:
- evidence: The email includes your EKM Push account key, which provides administrative access to your Push account and your meter data.
  how_to_obtain: Provided in the EKM Push account information email sent at purchase.
  location: query
  name: account key
  type: apiKey
slug: ekm-metering-authentication
source_filename: ekm-metering-authentication.yml
source_heading: Authentication Profile
source_url: https://help.ekmmetering.com/support/solutions/articles/6000256939-ekm-push3-installation-and-setup
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.ekmmetering.com/support/solutions/articles/6000256939-ekm-push3-installation-and-setup\nsources:\n- https://help.ekmmetering.com/support/solutions/articles/6000256939-ekm-push3-installation-and-setup\ndescription: Authentication uses an account key passed as a query parameter.\nschemes:\n- type: apiKey\n  name: account key\n  evidence: The email includes your EKM Push account key, which provides administrative access to your Push account and your meter data.\n  location: query\n  how_to_obtain: Provided in the EKM Push account information email sent at purchase.\ndocs: https://help.ekmmetering.com/support/solutions/articles/6000256939-ekm-push3-installation-and-setup\n"
source_yaml_url: https://artifacts.apis.io/ekm-metering/authentication/ekm-metering-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Submetering
- IoT
- Energy
- Utilities
- Cloud
---
