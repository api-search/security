---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: untuckit.com
  spf: true
hosts:
- cert_expires: Sep 22 13:20:02 2026 GMT
  host: untuckit.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Untuckit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UNTUCKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UNTUCKit
provider_slug: untuckit
slug: untuckit-domain-security
source_filename: untuckit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: untuckit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: untuckit.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/untuckit/refs/heads/main/security/untuckit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Apparel
- Retail
- eCommerce
- Shopify
- Agentic Commerce
- MCP
- UCP
---
