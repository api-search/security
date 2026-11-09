---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: activitysmith.com
  spf: true
hosts:
- cert_expires: Jan 22 07:06:11 2027 GMT
  host: activitysmith.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Activitysmith Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ActivitySmith, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ActivitySmith
provider_slug: activitysmith-com
slug: activitysmith-com-domain-security
source_filename: activitysmith-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: activitysmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 07:06:11 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: activitysmith.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/activitysmith-com/security/activitysmith-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile Notifications
- Live Activities
- AI Agent Integration
- Backend Monitoring
- Deployment Alerts
---
