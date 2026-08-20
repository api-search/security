---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:cert-request-l@monash.edu"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monash.edu
  spf: true
  x-operator: institution
- caa:
  - 0 issue "quovadisglobal.com"
  - 0 issuewild "quovadisglobal.com"
  - 0 issuewild "amazonaws.com"
  - 0 iodef "mailto:cert-request-l@monash.edu"
  - 0 issue "amazonaws.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: mailto:05clawtu@ag.dmarcian-ap.com
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: monash.edu.au
  note: Monash's Australian registrable domain, added 2026-08-19. It carries the identity federation surface (idp.monash.edu.au) and the eResearch HPC SP, and was absent from the previous revision even though the repo's most significant contract lives on it.
  spf: true
  spf_record: v=spf1 include:_spf.google.com -all
  x-operator: institution
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  edge: cloudflare
  host: www.monash.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'Returns HTTP 403 with cf-mitigated: challenge to non-browser clients — a Cloudflare managed bot challenge, not an outage. Live for browsers.'
  tls_version: TLSv1.3
  x-operator: institution
- cert_expires: Feb 26 23:59:59 2027 GMT
  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M01
  host: idp.monash.edu.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: Shibboleth IdP; serves signed SAML 2.0 metadata as application/xml.
  tls_version: TLSv1.3
  x-operator: institution
- cert_expires: Jan 31 23:59:59 2027 GMT
  cert_issuer: C=GB, O=Sectigo Limited, CN=Sectigo Public Server Authentication CA OV R36
  host: crams-api.erc.monash.edu
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: 'CRAMS portal. Sends x-frame-options: DENY, x-content-type-options: nosniff and referrer-policy: same-origin.'
  tls_version: TLSv1.3
  x-operator: institution
- cert_expires: Jan  2 23:59:59 2027 GMT
  cert_issuer: C=GB, O=Sectigo Limited, CN=Sectigo Public Server Authentication CA OV R36
  host: hpc.erc.monash.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
  x-operator: institution
- cert_expires: Oct 21 23:59:59 2026 GMT
  cert_issuer: C=AT, O=ZeroSSL GmbH, CN=ZeroSSL RSA DV SSL CA 2
  host: docs.erc.monash.edu
  hsts: false
  https: true
  note: Only institution host probed without HSTS, and the only one on a domain-validated certificate rather than an OV certificate.
  tls_version: TLSv1.3
  x-operator: institution
kind: domain-security
layout: security
method: probed
name: Monash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monash University, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Monash University
provider_slug: monash
slug: monash-domain-security
source_filename: monash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of the hosts and domains Monash University itself operates.\n  Rescoped 2026-08-19 by the university pipeline: the previous revision probed\n  api.figshare.com and the figshare.com domain and recorded the result as Monash's\n  security posture. Those are generic vendor hosts shared by every Figshare customer and\n  have been dropped — a vendor's TLS and DMARC configuration is not the institution's.\n  Only hosts under a Monash-owned registrable domain (monash.edu, monash.edu.au) are\n  probed here.\nscope:\n  included: institution-operated hosts only\n  excluded_vendor_hosts:\n  - host: api.figshare.com\n    reason: generic vendor host, shared by every Figshare customer\n  - host: monash.figshare.com\n    reason: tenant host on the Figshare platform; TLS terminated by the vendor\n  excluded_vendor_domains:\n  - domain: figshare.com\n    reason: vendor-controlled registrable domain\nhosts:\n- host:\
  \ www.monash.edu\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  edge: cloudflare\n  note: >-\n    Returns HTTP 403 with cf-mitigated: challenge to non-browser clients — a Cloudflare\n    managed bot challenge, not an outage. Live for browsers.\n- host: idp.monash.edu.au\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M01\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  note: Shibboleth IdP; serves signed SAML 2.0 metadata as application/xml.\n- host: crams-api.erc.monash.edu\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: C=GB, O=Sectigo Limited, CN=Sectigo Public Server Authentication CA OV R36\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  note:\
  \ >-\n    CRAMS portal. Sends x-frame-options: DENY, x-content-type-options: nosniff and\n    referrer-policy: same-origin.\n- host: hpc.erc.monash.edu.au\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: C=GB, O=Sectigo Limited, CN=Sectigo Public Server Authentication CA OV R36\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.erc.monash.edu\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: C=AT, O=ZeroSSL GmbH, CN=ZeroSSL RSA DV SSL CA 2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n  note: >-\n    Only institution host probed without HSTS, and the only one on a domain-validated\n    certificate rather than an OV certificate.\ndomains:\n- domain: monash.edu\n  x-operator: institution\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:cert-request-l@monash.edu\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"\
  amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: monash.edu.au\n  x-operator: institution\n  dnssec: false\n  caa:\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issuewild \"quovadisglobal.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 iodef \"mailto:cert-request-l@monash.edu\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: reject\n  dmarc_rua: mailto:05clawtu@ag.dmarcian-ap.com\n  note: >-\n    Monash's Australian registrable domain, added 2026-08-19. It carries the identity\n    federation surface (idp.monash.edu.au) and the eResearch HPC SP, and was absent from\n    the previous revision even though the repo's most significant contract lives on it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/security/monash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Australia
- Group of Eight
- Identity Federation
- Research Computing
- Research Repository
- Course Catalog
---
