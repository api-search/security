---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blackunicornfactory.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: followmeforequity.com
  spf: true
hosts:
- cert_expires: Oct 21 19:25:46 2026 GMT
  host: blackunicornfactory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 19:25:52 2026 GMT
  host: followmeforequity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Unicorn Factory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Unicorn Factory, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Black Unicorn Factory
provider_slug: black-unicorn-factory
slug: black-unicorn-factory-domain-security
source_filename: black-unicorn-factory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackunicornfactory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 19:25:46 2026 GMT\n  hsts: false\n- host: followmeforequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 19:25:52 2026 GMT\n  hsts: false\ndomains:\n- domain: blackunicornfactory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: followmeforequity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-unicorn-factory/refs/heads/main/security/black-unicorn-factory-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Venture Capital
- Pre-IPO
- Startup Accelerator
- Direct Listing
- Equity
- Private Markets
---
