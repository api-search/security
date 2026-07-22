---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lovys.com
  spf: true
hosts:
- cert_expires: Sep 29 20:53:53 2026 GMT
  host: lovys.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lovys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lovys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lovys
provider_slug: lovys
slug: lovys-domain-security
source_filename: lovys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lovys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:53:53 2026 GMT\n  hsts: false\ndomains:\n- domain: lovys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovys/refs/heads/main/security/lovys-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Insurtech
- Embedded Insurance
- Partner API
- Home Insurance
- Pet Insurance
- Smartphone Insurance
- OAuth2
- Azure API Management
---
