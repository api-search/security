---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudqix.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: staging2.cloudqix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudqix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudQix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CloudQix
provider_slug: cloudqix
slug: cloudqix-domain-security
source_filename: cloudqix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: staging2.cloudqix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudqix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudqix/refs/heads/main/security/cloudqix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- iPaaS
- Integration
- Automation
- API
---
