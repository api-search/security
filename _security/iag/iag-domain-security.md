---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc.reporting@iag.com.au
  dnssec: false
  domain: iag.com.au
  spf: true
  spf_record: v=spf1 include:_spf.salesforce.com include:spf.protection.outlook.com a:chi-web-01.simprocloud.com include:eventsairmail.com include:service-now.com include:_spf-dc10.sapsf.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc.reporting@iag.com.au
  dnssec: false
  domain: cgu.com.au
  note: SPF includes mrspf.ebix.com.au and a:ssiw.qvalent.com — independent corroboration that CGU transacts over the Ebix Sunrise Exchange broker rail and uses Qvalent (Westpac) payment infrastructure.
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc.reporting@iag.com.au
  dnssec: false
  domain: nrma.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc.reporting@iag.com.au
  dnssec: false
  domain: wfi.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc.reporting@iag.com.au
  dnssec: false
  domain: iag.co.nz
  note: SPF terminates in ~all (softfail) rather than -all as on the Australian domains.
  spf: true
  spf_qualifier: softfail
- caa: []
  dmarc: false
  dnssec: false
  domain: rollin.com.au
  note: ROLLiN' brand domain. The _dmarc TXT record contains an SPF string, not a DMARC policy — a misconfiguration that leaves the domain without a valid DMARC record. The SPF itself authorises only an RFC 4193 unique-local IPv6 range, which cannot originate internet mail.
  spf: true
  spf_record: v=spf1 ip6:fdcf:abda:4154::/48 -all
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  edge: Akamai
  host: www.iag.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  edge: Akamai
  host: apis.iag.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 403
  https: true
  note: Host resolves via apis.iag.com.au.edgekey.net. Returns Akamai "Access Denied" for every path.
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  edge: Azure App Service
  host: docs.iag.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: CNAME docs-iag-prod-wap.azurewebsites.net. Redirects to Microsoft Entra ID sign-in via Azure Easy Auth. Internal documentation behind SSO.
  tls_version: TLSv1.3
- cert_expires: Aug 12 23:59:59 2026 GMT
  edge: Apigee Edge
  host: api.iag.com.au
  hsts: true
  hsts_max_age: 86400
  https: true
  note: CNAME iag-prod-production.apigee.net. Virtual host https_vhost.
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  edge: Apigee Edge
  host: api.cgu.com.au
  hsts: true
  hsts_max_age: 86400
  https: true
  note: CNAME iag-prod-production.apigee.net. Virtual host https_cgu_vhost.
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  edge: Apigee Edge
  host: api.nrma.com.au
  hsts: true
  hsts_max_age: 86400
  https: true
  note: CNAME iag-prod-production.apigee.net. Virtual host https_nrma_vhost.
  tls_version: TLSv1.2
- cert_expires: Dec  3 23:59:59 2026 GMT
  edge: Apigee Edge
  host: api.wfi.com.au
  hsts: true
  hsts_max_age: 86400
  https: true
  note: Virtual host https_wfi_vhost. Fourth brand virtual host, newly identified this round.
  tls_version: TLSv1.2
- cert_expires: Dec  3 23:59:59 2026 GMT
  edge: Apigee Edge
  host: test-api.iag.com.au
  hsts: true
  hsts_max_age: 86400
  https: true
  note: CNAME iag-nonprod-test.apigee.net. Non-production Apigee organisation (iag-nonprod, env test), publicly resolvable. Newly identified this round.
  tls_version: TLSv1.2
- cert_expires: Oct 17 23:59:59 2026 GMT
  edge: Akamai
  host: api.iag.co.nz
  hsts: false
  https: true
  note: New Zealand business (State/AMI/NZI). Akamai "Access Denied"; no public content.
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  edge: Akamai
  host: www.cgu.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  edge: Akamai
  host: www.nrma.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  edge: Akamai
  host: www.iag.co.nz
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- host: security.iag.com.au
  hsts: false
  http_status: 401
  https: true
  note: HTTP 401 with WWW-Authenticate Basic realm "IBM Verify Identity Access for Web". An IBM Verify Identity Access (WebSEAL) reverse proxy, not a public security page.
kind: domain-security
layout: security
method: probed
name: Iag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insurance Australia Group, probed live across 13 host(s) and 6 registrable domain(s). 13 host(s) serve HTTPS (up to TLSv1.3); 9 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Insurance Australia Group
provider_slug: iag
slug: iag-domain-security
source_filename: iag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every IAG brand website, Apigee gateway virtual host and ancillary host\nsummary: >-\n  Every IAG host is HTTPS-only and presents a valid certificate. The estate\n  splits cleanly in two: the Akamai-fronted brand websites negotiate TLS 1.3,\n  while all five Apigee gateway virtual hosts negotiate TLS 1.2. HSTS is present\n  everywhere except api.iag.co.nz, but the max-age is weak (86400 = 1 day) on\n  every Apigee host and on the NRMA, CGU and IAG NZ brand sites; only\n  apis.iag.com.au and docs.iag.com.au set a one-year max-age with\n  includeSubDomains, and only apis.iag.com.au sets preload. No IAG domain is\n  DNSSEC-signed and no IAG domain publishes a CAA record. Email authentication is\n  strong and centrally managed — every domain publishes SPF and a DMARC record\n  with p=reject reporting to dmarc.reporting@iag.com.au.\nhosts:\n- host: www.iag.com.au\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: 'Dec  6 23:59:59 2026 GMT'\n  hsts: false\n  edge: Akamai\n- host: apis.iag.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct  3 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 403\n  edge: Akamai\n  note: Host resolves via apis.iag.com.au.edgekey.net. Returns Akamai \"Access Denied\" for every path.\n- host: docs.iag.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Dec 13 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  edge: Azure App Service\n  note: >-\n    CNAME docs-iag-prod-wap.azurewebsites.net. Redirects to Microsoft Entra ID\n    sign-in via Azure Easy Auth. Internal documentation behind SSO.\n- host: api.iag.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: 'Aug 12 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 86400\n  edge: Apigee Edge\n  note: CNAME iag-prod-production.apigee.net.\
  \ Virtual host https_vhost.\n- host: api.cgu.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: 'Sep 18 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 86400\n  edge: Apigee Edge\n  note: CNAME iag-prod-production.apigee.net. Virtual host https_cgu_vhost.\n- host: api.nrma.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: 'Sep 18 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 86400\n  edge: Apigee Edge\n  note: CNAME iag-prod-production.apigee.net. Virtual host https_nrma_vhost.\n- host: api.wfi.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: 'Dec  3 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 86400\n  edge: Apigee Edge\n  note: Virtual host https_wfi_vhost. Fourth brand virtual host, newly identified this round.\n- host: test-api.iag.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: 'Dec  3 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 86400\n  edge: Apigee Edge\n  note: >-\n    CNAME iag-nonprod-test.apigee.net. Non-production\
  \ Apigee organisation\n    (iag-nonprod, env test), publicly resolvable. Newly identified this round.\n- host: api.iag.co.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct 17 23:59:59 2026 GMT'\n  hsts: false\n  edge: Akamai\n  note: New Zealand business (State/AMI/NZI). Akamai \"Access Denied\"; no public content.\n- host: www.cgu.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Dec  6 23:59:59 2026 GMT'\n  hsts: false\n  edge: Akamai\n- host: www.nrma.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Dec  6 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 86400\n  hsts_include_subdomains: true\n  edge: Akamai\n- host: www.iag.co.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct 17 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 86400\n  hsts_include_subdomains: true\n  edge: Akamai\n- host: security.iag.com.au\n  https: true\n  http_status: 401\n  hsts: false\n  note: >-\n    HTTP 401 with WWW-Authenticate Basic realm \"IBM\
  \ Verify Identity Access for\n    Web\". An IBM Verify Identity Access (WebSEAL) reverse proxy, not a public\n    security page.\ndomains:\n- domain: iag.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.salesforce.com include:spf.protection.outlook.com a:chi-web-01.simprocloud.com include:eventsairmail.com include:service-now.com include:_spf-dc10.sapsf.com -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc.reporting@iag.com.au\n- domain: cgu.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc.reporting@iag.com.au\n  note: >-\n    SPF includes mrspf.ebix.com.au and a:ssiw.qvalent.com — independent\n    corroboration that CGU transacts over the Ebix Sunrise Exchange broker rail\n    and uses Qvalent (Westpac) payment infrastructure.\n- domain: nrma.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc.reporting@iag.com.au\n- domain: wfi.com.au\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc.reporting@iag.com.au\n- domain: iag.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  spf_qualifier: softfail\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc.reporting@iag.com.au\n  note: SPF terminates in ~all (softfail) rather than -all as on the Australian domains.\n- domain: rollin.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 ip6:fdcf:abda:4154::/48 -all\n  dmarc: false\n  note: >-\n    ROLLiN' brand domain. The _dmarc TXT record contains an SPF string, not a\n    DMARC policy — a misconfiguration that leaves the domain without a valid\n    DMARC record. The SPF itself authorises only an RFC 4193 unique-local IPv6\n    range, which cannot originate internet mail.\nfindings:\n- No IAG domain is DNSSEC-signed.\n- No IAG domain publishes a CAA record.\n- All five Apigee virtual hosts negotiate TLS 1.2, not TLS 1.3.\n- HSTS max-age of 86400 on the Apigee\
  \ hosts is an order of magnitude below the\n  31536000 recommended for preload eligibility.\n- _dmarc.rollin.com.au contains an SPF record instead of a DMARC policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iag/refs/heads/main/security/iag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- New Zealand
- Property and Casualty
- General Insurance
- Carrier
- Underwriting
- Claims
- Broker
- Partner Gated
---
