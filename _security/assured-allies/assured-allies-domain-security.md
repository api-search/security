---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: assuredallies.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:_spf.salesforce.com include:4871571.spf04.hubspotemail.net -all
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neverstop.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:4871571.spf04.hubspotemail.net include:_spf.salesforce.com include:mailgun.org -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: assured.care
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com ~all
hosts:
- cert_expires: Sep 11 15:58:19 2026 GMT
  host: assuredallies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 08:39:35 2026 GMT
  host: neverstop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 04:48:19 2026 GMT
  host: app.neverstop.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 08:40:35 2026 GMT
  host: assured.care
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 0
  hsts_preload: true
  https: true
  note: Strict-Transport-Security is served with max-age=0, which disables HSTS enforcement despite the includeSubDomains/preload directives.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Assured Allies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assured Allies, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Assured Allies
provider_slug: assured-allies
slug: assured-allies-domain-security
source_filename: assured-allies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (website + both member-platform domains)\nhosts:\n- host: assuredallies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:58:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: neverstop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:39:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.neverstop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 04:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: assured.care\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:40:35 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: 'Strict-Transport-Security is served with max-age=0, which disables HSTS enforcement\n    despite the includeSubDomains/preload directives.'\ndomains:\n\
  - domain: assuredallies.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:_spf.salesforce.com\n    include:4871571.spf04.hubspotemail.net -all\n  dmarc: true\n  dmarc_policy: reject\n- domain: neverstop.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:4871571.spf04.hubspotemail.net\n    include:_spf.salesforce.com include:mailgun.org -all\n  dmarc: true\n  dmarc_policy: reject\n\
  - domain: assured.care\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com ~all\n  dmarc: true\n  dmarc_policy: reject\nx-ownership-evidence:\n  note: The three domains share DMARC aggregate-report mailboxes, corroborating common\n    ownership of assuredallies.com, neverstop.com and assured.care.\n  shared_rua:\n  - 4b7a125b51@rua.easydmarc.us (all three domains)\n  - d56dde6ef94f4cd390971a62cd492939@dmarc-reports.cloudflare.net (assuredallies.com\n    + assured.care)\nx-evidence:\n  probed: '2026-08-02'\n  tools:\n  - dig\n  - openssl s_client\n  - curl -I\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assured-allies/refs/heads/main/security/assured-allies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Insurtech
- Long-Term Care
- Health
- Aging
- Retirement
- Underwriting
- Wellness
---
