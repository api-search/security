---
api_specs:
- filename: uptimerobot-alert-contacts-api-openapi.yml
  format: yaml
  label: UptimeRobot Alert Contacts API
  slug: uptimerobot-alert-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-alert-contacts-api-openapi.yml
- filename: uptimerobot-incidents-api-openapi.yml
  format: yaml
  label: UptimeRobot Incidents API
  slug: uptimerobot-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-incidents-api-openapi.yml
- filename: uptimerobot-integrations-api-openapi.yml
  format: yaml
  label: UptimeRobot Integrations API
  slug: uptimerobot-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-integrations-api-openapi.yml
- filename: uptimerobot-maintenance-windows-api-openapi.yml
  format: yaml
  label: UptimeRobot Maintenance Windows API
  slug: uptimerobot-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-maintenance-windows-api-openapi.yml
- filename: uptimerobot-monitor-groups-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitor Groups API
  slug: uptimerobot-monitor-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitor-groups-api-openapi.yml
- filename: uptimerobot-monitors-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitors API
  slug: uptimerobot-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitors-api-openapi.yml
- filename: uptimerobot-monitors-bulk-operations-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitors - Bulk Operations API
  slug: uptimerobot-monitors-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitors-bulk-operations-api-openapi.yml
- filename: uptimerobot-psp-announcements-api-openapi.yml
  format: yaml
  label: UptimeRobot PSP Announcements API
  slug: uptimerobot-psp-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-psp-announcements-api-openapi.yml
- filename: uptimerobot-public-status-pages-api-openapi.yml
  format: yaml
  label: UptimeRobot Public Status Pages API
  slug: uptimerobot-public-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-public-status-pages-api-openapi.yml
- filename: uptimerobot-storm-protection-api-openapi.yml
  format: yaml
  label: UptimeRobot Storm Protection API
  slug: uptimerobot-storm-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-storm-protection-api-openapi.yml
- filename: uptimerobot-tags-api-openapi.yml
  format: yaml
  label: UptimeRobot Tags API
  slug: uptimerobot-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-tags-api-openapi.yml
- filename: uptimerobot-user-api-openapi.yml
  format: yaml
  label: UptimeRobot User API
  slug: uptimerobot-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uptimerobot.com
  spf: true
hosts:
- cert_expires: Jan 10 16:47:18 2027 GMT
  host: uptimerobot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uptimerobot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UptimeRobot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: UptimeRobot
provider_slug: uptimerobot
slug: uptimerobot-domain-security
source_filename: uptimerobot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptimerobot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 16:47:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uptimerobot.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/security/uptimerobot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Uptime Monitoring
- Status Pages
- Incident Management
- DevOps
- Monitoring Integrations
---
