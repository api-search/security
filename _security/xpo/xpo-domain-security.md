---
description: ''
domains:
- caa:
  - 0 iodef "mailto:networkteamengineering@xpo.com"
  - 0 issue "digicert.com; account=d55e1707fe59cbbcecc371e9b7ddadbdaf2e3ccbb4bac1f5ae6a686a8e26f25f"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xpo.com
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.xpo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xpo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XPO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: XPO
provider_slug: xpo
slug: xpo-domain-security
source_filename: xpo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xpo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: xpo.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:networkteamengineering@xpo.com\"\n  - 0 issue \"digicert.com; account=d55e1707fe59cbbcecc371e9b7ddadbdaf2e3ccbb4bac1f5ae6a686a8e26f25f\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xpo/refs/heads/main/security/xpo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fortune 500
- Freight
- Less-Than-Truckload
- Logistics
- Transportation
- Trucking
---
