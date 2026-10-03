---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boldlog.com
  spf: true
hosts:
- cert_expires: Dec 25 00:54:07 2026 GMT
  host: boldlog.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bold9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bold9, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bold9
provider_slug: bold9
slug: bold9-domain-security
source_filename: bold9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boldlog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 00:54:07 2026 GMT\n  hsts: false\ndomains:\n- domain: boldlog.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bold9/refs/heads/main/security/bold9-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Investment
- Marketplace
- Private-Equity
---
