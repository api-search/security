---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 iodef "mailto:contact@shibboleth.net"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shibboleth.net
  spf: true
hosts:
- cert_expires: Dec  8 11:36:50 2026 GMT
  host: www.shibboleth.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shibboleth Consortium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shibboleth Consortium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shibboleth Consortium
provider_slug: shibboleth-consortium
slug: shibboleth-consortium-domain-security
source_filename: shibboleth-consortium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shibboleth.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 11:36:50 2026 GMT\n  hsts: false\ndomains:\n- domain: shibboleth.net\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:contact@shibboleth.net\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shibboleth-consortium/refs/heads/main/security/shibboleth-consortium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Organization
- Identity
- Federation
- OpenSource
- NonProfit
---
