---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1;p=quarantine;pct=100;rua=mailto:dmarc-reports@parsleyhealth.com
  dnssec: false
  domain: parsleyhealth.com
  spf: true
  spf_record: v=spf1 include:helpscoutemail.com include:_spf.google.com include:sendgrid.net include:shops.shopify.com include:mailgun.org ~all
hosts:
- cert_expires: Oct  3 22:23:12 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  host: www.parsleyhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:26:32 2026 GMT
  cert_issuer: Let's Encrypt (YE1)
  host: store.parsleyhealth.com
  hsts: true
  hsts_header: max-age=7889238
  https: true
  note: Shopify-hosted storefront. Carries the only live machine surfaces on this company — the UCP/MCP endpoint and the Storefront GraphQL endpoint.
  tls_version: TLSv1.3
- cert_expires: Oct  1 16:44:48 2026 GMT
  cert_issuer: Let's Encrypt (YE2)
  host: help.parsleyhealth.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  https: true
  note: Help Scout Docs help centre.
  tls_version: TLSv1.3
- cert_expires: Sep 28 04:18:48 2026 GMT
  host: my.parsleyhealth.com
  hsts: false
  https: true
  note: authenticated member application (Google Frontend); no HSTS response header observed
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:14:35 2026 GMT
  host: app.parsleyhealth.com
  hsts: false
  https: true
  note: authenticated member application (Google Frontend); no HSTS response header observed
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsley Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsley Health, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parsley Health
provider_slug: parsley-health
slug: parsley-health-domain-security
source_filename: parsley-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Parsley Health host (2026-08-15; supersedes 2026-08-02)\nnote: >-\n  Re-probed and extended. Two findings changed since the 2026-08-02 pass. First, two hosts\n  previously recorded as \"does not resolve\" actually publish DANGLING CNAME records\n  pointing at deprovisioned infrastructure — api.parsleyhealth.com at a dead Aptible load\n  balancer and docs.parsleyhealth.com at a CloudFront distribution with no addresses. Both\n  are advertised in DNS with nothing behind them. Second, two hosts the earlier pass never\n  saw were added: store.parsleyhealth.com (Shopify) and help.parsleyhealth.com (Help\n  Scout), and both, unlike the marketing site, do send HSTS. The apex marketing site still\n  sends no HSTS header and the zone is still unsigned.\nhosts:\n- host: www.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WR3)\n  cert_expires: Oct  3 22:23:12\
  \ 2026 GMT\n  hsts: false\n- host: store.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (YE1)\n  cert_expires: Oct 28 23:26:32 2026 GMT\n  hsts: true\n  hsts_header: max-age=7889238\n  note: >-\n    Shopify-hosted storefront. Carries the only live machine surfaces on this company —\n    the UCP/MCP endpoint and the Storefront GraphQL endpoint.\n- host: help.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (YE2)\n  cert_expires: Oct  1 16:44:48 2026 GMT\n  hsts: true\n  hsts_header: max-age=31536000; includeSubDomains; preload\n  note: Help Scout Docs help centre.\n- host: my.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:18:48 2026 GMT\n  hsts: false\n  note: authenticated member application (Google Frontend); no HSTS response header observed\n- host: app.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:14:35 2026 GMT\n  hsts: false\n  note:\
  \ authenticated member application (Google Frontend); no HSTS response header observed\ndangling_cnames:\n- host: api.parsleyhealth.com\n  cname: elb-parsley-17779.aptible.in\n  target_dns_status: NXDOMAIN\n  severity_note: >-\n    A CNAME is published for a hostname whose target no longer exists. Nothing answers on\n    this name today. Recorded as an observed DNS fact; no takeover attempt was made and\n    none should be. Withdrawing the record is the provider's fix.\n  probed: '2026-08-15'\n- host: docs.parsleyhealth.com\n  cname: d3sqky83ufbfgj.cloudfront.net\n  target_dns_status: NOERROR, no address records\n  severity_note: >-\n    CNAME published for a CloudFront distribution that returns no addresses. Same posture\n    and same fix as api.parsleyhealth.com.\n  probed: '2026-08-15'\ndomains:\n- domain: parsleyhealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\
  \n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  spf_record: 'v=spf1 include:helpscoutemail.com include:_spf.google.com include:sendgrid.net include:shops.shopify.com include:mailgun.org ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1;p=quarantine;pct=100;rua=mailto:dmarc-reports@parsleyhealth.com'\nsecurity_txt:\n  published: false\n  probed_hosts: [www.parsleyhealth.com, store.parsleyhealth.com, help.parsleyhealth.com]\n  result: 404 on all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsley-health/refs/heads/main/security/parsley-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Telehealth
- Telemedicine
- Functional Medicine
- Primary Care
- Wellness
- Nutrition
- Diagnostics
- Lab Testing
- Membership
- Digital Health
- Consumer Health
- E-Commerce
- Agentic Commerce
- MCP
- Supplements
---
