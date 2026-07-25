---
api_specs:
- filename: teamcity-agent-pools-api-openapi.yml
  format: yaml
  label: TeamCity Agent Pools API
  slug: teamcity-agent-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-agent-pools-api-openapi.yml
- filename: teamcity-agents-api-openapi.yml
  format: yaml
  label: TeamCity Agents API
  slug: teamcity-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-agents-api-openapi.yml
- filename: teamcity-audit-api-openapi.yml
  format: yaml
  label: TeamCity Audit API
  slug: teamcity-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-audit-api-openapi.yml
- filename: teamcity-build-configurations-api-openapi.yml
  format: yaml
  label: TeamCity Build Configurations API
  slug: teamcity-build-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-build-configurations-api-openapi.yml
- filename: teamcity-build-queue-api-openapi.yml
  format: yaml
  label: TeamCity Build Queue API
  slug: teamcity-build-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-build-queue-api-openapi.yml
- filename: teamcity-builds-api-openapi.yml
  format: yaml
  label: TeamCity Builds API
  slug: teamcity-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-builds-api-openapi.yml
- filename: teamcity-changes-api-openapi.yml
  format: yaml
  label: TeamCity Changes API
  slug: teamcity-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-changes-api-openapi.yml
- filename: teamcity-cloud-api-openapi.yml
  format: yaml
  label: TeamCity Cloud API
  slug: teamcity-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-cloud-api-openapi.yml
- filename: teamcity-investigations-api-openapi.yml
  format: yaml
  label: TeamCity Investigations API
  slug: teamcity-investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-investigations-api-openapi.yml
- filename: teamcity-mutes-api-openapi.yml
  format: yaml
  label: TeamCity Mutes API
  slug: teamcity-mutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-mutes-api-openapi.yml
- filename: teamcity-problems-api-openapi.yml
  format: yaml
  label: TeamCity Problems API
  slug: teamcity-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-problems-api-openapi.yml
- filename: teamcity-projects-api-openapi.yml
  format: yaml
  label: TeamCity Projects API
  slug: teamcity-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-projects-api-openapi.yml
- filename: teamcity-server-api-openapi.yml
  format: yaml
  label: TeamCity Server API
  slug: teamcity-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-server-api-openapi.yml
- filename: teamcity-tests-api-openapi.yml
  format: yaml
  label: TeamCity Tests API
  slug: teamcity-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-tests-api-openapi.yml
- filename: teamcity-user-groups-api-openapi.yml
  format: yaml
  label: TeamCity User Groups API
  slug: teamcity-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-user-groups-api-openapi.yml
- filename: teamcity-users-api-openapi.yml
  format: yaml
  label: TeamCity Users API
  slug: teamcity-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-users-api-openapi.yml
- filename: teamcity-vcs-roots-api-openapi.yml
  format: yaml
  label: TeamCity VCS Roots API
  slug: teamcity-vcs-roots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-vcs-roots-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetbrains.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.jetbrains.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teamcity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeamCity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TeamCity
provider_slug: teamcity
slug: teamcity-domain-security
source_filename: teamcity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetbrains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jetbrains.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/security/teamcity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Build Automation
- CI/CD
- Continuous Integration
- Deployment
- DevOps
- Testing
---
