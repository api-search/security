---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nexamp.com
  spf: true
hosts:
- cert_expires: Sep 13 12:58:07 2026 GMT
  host: www.nexamp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: community.nexamp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 12:58:07 2026 GMT
  host: portal.nexamp.com
  https: true
  note: Nexamp Decarbonization Platform login (Cloudflare-fronted); manually probed, not an apis.yml Website/Portal host at probe time
  tls_version: TLSv1.3
- cert_expires: May 14 23:59:59 2024 GMT
  cert_issuer: Sectigo RSA Domain Validation Secure Server CA
  cert_not_before: Apr 14 00:00:00 2023 GMT
  cert_subject: CN=*.nexamp.com
  cert_valid: false
  finding: EXPIRED TLS CERTIFICATE — the wildcard *.nexamp.com certificate served by api.nexamp.com expired 2024-05-14. Any standards-compliant TLS client fails the handshake (curl reports an "SSL certificate problem - certificate has expired" error) unless verification is disabled. Observed 2026-08-01.
  host: api.nexamp.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Undocumented API host (Azure App Service, nexamp-api-production.azurewebsites.net). Root and most paths 302 to login.microsoftonline.com (Microsoft Entra ID); /openapi.json, /swagger.json and /.well-known/* return 401. Manually probed with certificate verification disabled; not advertised as a public developer API.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexamp, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Nexamp
provider_slug: nexamp
slug: nexamp-domain-security
source_filename: nexamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 12:58:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: community.nexamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.nexamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 12:58:07 2026 GMT\n  note: Nexamp Decarbonization Platform login (Cloudflare-fronted); manually probed,\n    not an apis.yml Website/Portal host at probe time\n- host: api.nexamp.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 2592000\n  cert_subject: CN=*.nexamp.com\n  cert_issuer: Sectigo RSA Domain Validation Secure Server CA\n  cert_not_before: Apr 14 00:00:00 2023 GMT\n  cert_expires: May 14 23:59:59 2024 GMT\n  cert_valid: false\n  finding: >-\n    EXPIRED\
  \ TLS CERTIFICATE — the wildcard *.nexamp.com certificate served by\n    api.nexamp.com expired 2024-05-14. Any standards-compliant TLS client fails\n    the handshake (curl reports an \"SSL certificate problem - certificate has\n    expired\" error) unless verification is disabled. Observed 2026-08-01.\n  note: >-\n    Undocumented API host (Azure App Service, nexamp-api-production.azurewebsites.net).\n    Root and most paths 302 to login.microsoftonline.com (Microsoft Entra ID);\n    /openapi.json, /swagger.json and /.well-known/* return 401. Manually probed with\n    certificate verification disabled; not advertised as a public developer API.\ndomains:\n- domain: nexamp.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexamp/refs/heads/main/security/nexamp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Solar
- Clean Energy
- Community Solar
- Renewable Energy
- Energy Storage
- Sustainability
- Utilities
---
