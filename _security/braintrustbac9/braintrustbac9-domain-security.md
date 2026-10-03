---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: usebraintrust.com
  spf: true
hosts:
- cert_expires: Oct 31 16:37:23 2026 GMT
  host: www.usebraintrust.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Braintrustbac9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braintrustbac9, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Braintrustbac9
provider_slug: braintrustbac9
slug: braintrustbac9-domain-security
source_filename: braintrustbac9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usebraintrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 16:37:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usebraintrust.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintrustbac9/refs/heads/main/security/braintrustbac9-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Talent Marketplace
- AI Recruiting
- Enterprise Hiring
- Workflow Automation
- Human Data Infrastructure
---
