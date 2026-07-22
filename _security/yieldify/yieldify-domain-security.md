---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yieldify.com
  spf: true
hosts:
- cert_expires: Oct  8 08:04:08 2026 GMT
  host: yieldify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yieldify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yieldify *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yieldify *
provider_slug: yieldify
slug: yieldify-domain-security
source_filename: yieldify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yieldify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:04:08 2026 GMT\n  hsts: false\ndomains:\n- domain: yieldify.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yieldify/refs/heads/main/security/yieldify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Personalization
- Conversion Rate Optimization
- Ecommerce
- Marketing Technology
- Customer Experience
---
