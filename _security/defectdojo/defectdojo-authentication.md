---
anonymous_access: false
api_key_in: []
api_specs:
- filename: defectdojo-openapi-generated.yml
  format: yaml
  label: DefectDojo API
  slug: defectdojo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defectdojo/openapi/_ae-authored/defectdojo-openapi-generated.yml
auth_types: []
description: DefectDojo authentication methods as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DefectDojo Authentication
name_suffix: Authentication
oauth_flows: []
overview: DefectDojo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DefectDojo
provider_slug: defectdojo
scheme_count: 2
schemes:
- evidence: DefectDojo Pro can authenticate users from headers set by a trusted reverse proxy in front of DefectDojo — the pattern usually called remote user or header authentication.
  header: REMOTE_USER
  how_to_obtain: Configure the environment variable DD_AUTH_REMOTEUSER_USERNAME_HEADER (default REMOTE_USER) on the DefectDojo instance and ensure a trusted reverse proxy injects that header with the username on each request.
  location: header
  name: Remote User Header
  type: other
- evidence: DefectDojo Pro supports LDAP authentication from Connect > Authorization > Providers — no custom Docker images or configuration files are required. Unlike the other providers on this page, LDAP is not a redirect-based flow. Users sign in with the standard DefectDojo username and password form, and their credentials are checked against your directory.
  header: Authorization
  how_to_obtain: Configure LDAP provider in DefectDojo UI with server URI, bind DN, bind password, and attribute mappings; users then authenticate using their LDAP username and password via the standard login form.
  location: header
  name: LDAP
  type: http-basic
slug: defectdojo-authentication
source_filename: defectdojo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.defectdojo.com/get_started/pro/onprem/passwordless_database/
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.defectdojo.com/get_started/pro/onprem/passwordless_database/\nsources:\n- https://docs.defectdojo.com/get_started/pro/onprem/passwordless_database/\n- https://docs.defectdojo.com/admin/user_management/pro__mfa/\n- https://docs.defectdojo.com/admin/sso/pro__remote_user/\n- https://docs.defectdojo.com/admin/sso/pro__ldap/\ndescription: DefectDojo authentication methods as documented\nschemes:\n- type: other\n  name: Remote User Header\n  evidence: DefectDojo Pro can authenticate users from headers set by a trusted reverse proxy in front of DefectDojo — the pattern usually called\n    remote user or header authentication.\n  location: header\n  header: REMOTE_USER\n  how_to_obtain: Configure the environment variable DD_AUTH_REMOTEUSER_USERNAME_HEADER (default REMOTE_USER) on the DefectDojo instance and ensure\n    a trusted reverse proxy injects that header with the username\
  \ on each request.\n- type: http-basic\n  name: LDAP\n  evidence: DefectDojo Pro supports LDAP authentication from Connect > Authorization > Providers — no custom Docker images or configuration files\n    are required. Unlike the other providers on this page, LDAP is not a redirect-based flow. Users sign in with the standard DefectDojo username\n    and password form, and their credentials are checked against your directory.\n  location: header\n  header: Authorization\n  how_to_obtain: Configure LDAP provider in DefectDojo UI with server URI, bind DN, bind password, and attribute mappings; users then authenticate\n    using their LDAP username and password via the standard login form.\ndocs: https://docs.defectdojo.com/get_started/pro/onprem/passwordless_database/\n"
source_yaml_url: https://artifacts.apis.io/defectdojo/authentication/defectdojo-authentication.yml
summary_line: 2 schemes
tags:
- Vulnerability Management
- Application Security
- DevSecOps
- Compliance
- Penetration Testing
- SOC
- psirt
- Cloud Security
---
