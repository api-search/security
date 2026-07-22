---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@meetfabric.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meetfabric.com
  spf: true
hosts:
- cert_expires: Sep  6 15:09:22 2026 GMT
  host: meetfabric.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fabric Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fabric Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fabric Technologies
provider_slug: fabric-technologies
slug: fabric-technologies-domain-security
source_filename: fabric-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meetfabric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:09:22 2026 GMT\n  hsts: null\ndomains:\n- domain: meetfabric.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@meetfabric.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric-technologies/refs/heads/main/security/fabric-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Insurance
- Life Insurance
- Financial Services
- Estate Planning
- Investing
- Wills
---
