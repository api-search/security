---
api_specs:
- filename: lithium-care-conversation-api-v2-openapi.json
  format: json
  label: Khoros Care API
  slug: care
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-care-conversation-api-v2-openapi.json
- filename: lithium-marketing-conversations-openapi.json
  format: json
  label: Khoros Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-marketing-conversations-openapi.json
- filename: lithium-flow-flow-rest-api-openapi.json
  format: json
  label: Khoros Flow API
  slug: flow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-flow-flow-rest-api-openapi.json
description: Live TLS/DNS posture across the Khoros, Lithium, Spredfast and flow.ai hosts this provider spans. The headline finding is that the legacy lithium.com apex — still the company's original domain and still serving the Khoros marketing site — presents a TLS certificate that expired on 3 January 2026, so every modern client refuses the connection. HSTS coverage is inconsistent and no domain in the estate is DNSSEC-signed.
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: khoros.ai
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: khoros.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lithium.com
  note: DMARC reporting handled by Proofpoint. No CAA records.
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spredfast.com
  note: DMARC reporting handled by Proofpoint. No CAA records.
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:max@flow.ai"
  - 0 iodef "mailto:gijs@flow.ai"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flow.ai
  spf: true
hosts:
- cert_expires: Sep  3 05:48:31 2026 GMT
  host: khoros.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:18:28 2026 GMT
  host: developer.khoros.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.app.lithium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expired: true
  cert_expires: Jan  3 19:44:37 2026 GMT
  host: www.lithium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Certificate expired 2026-01-03; TLS handshake fails certificate validation. Serves the Khoros marketing site when validation is bypassed.
  tls_version: null
- cert_expired: true
  cert_expires: Jan  3 19:44:37 2026 GMT
  host: lithium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Same expired certificate as www.lithium.com. HSTS is asserted, which makes the failure non-bypassable in browsers.
  tls_version: null
- cert_expires: Aug 25 18:51:00 2026 GMT
  host: community.khoros.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.spredfast.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: login.spredfast.com
  hsts: false
  https: true
  note: Khoros Marketing OAuth authorization server — no HSTS.
  tls_version: TLSv1.3
- cert_expires: Oct 13 15:18:06 2026 GMT
  host: api.flow.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.massrelevance.com
  hsts: false
  https: true
  note: Khoros Marketing Stream API host.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lithium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lithium, probed live across 10 host(s) and 5 registrable domain(s). 10 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lithium
provider_slug: lithium
slug: lithium-domain-security
source_filename: lithium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: khoros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:48:31 2026 GMT\n  hsts: false\n- host: developer.khoros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.app.lithium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\n- host: www.lithium.com\n  https: true\n  tls_version: null\n  cert_expires: Jan  3 19:44:37 2026 GMT\n  cert_expired: true\n  hsts: true\n  hsts_max_age: 31536000\n  note: Certificate expired 2026-01-03; TLS handshake fails certificate validation. Serves the Khoros\n    marketing site when validation is bypassed.\n- host: lithium.com\n  https: true\n  tls_version: null\n  cert_expires: Jan  3 19:44:37 2026 GMT\n  cert_expired: true\n  hsts: true\n  hsts_max_age: 31536000\n  note: Same\
  \ expired certificate as www.lithium.com. HSTS is asserted, which makes the failure non-bypassable\n    in browsers.\n- host: community.khoros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:51:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.spredfast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n- host: login.spredfast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n  note: Khoros Marketing OAuth authorization server — no HSTS.\n- host: api.flow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 15:18:06 2026 GMT\n  hsts: false\n- host: api.massrelevance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: false\n  note: Khoros Marketing Stream API host.\ndomains:\n- domain: khoros.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n- domain: khoros.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lithium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: DMARC reporting handled by Proofpoint. No CAA records.\n- domain: spredfast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: DMARC reporting handled by Proofpoint. No CAA records.\n- domain: flow.ai\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"\
  letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:max@flow.ai\"\n  - 0 iodef \"mailto:gijs@flow.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\ndescription: Live TLS/DNS posture across the Khoros, Lithium, Spredfast and flow.ai hosts this provider\n  spans. The headline finding is that the legacy lithium.com apex — still the company's original domain\n  and still serving the Khoros marketing site — presents a TLS certificate that expired on 3 January 2026,\n  so every modern client refuses the connection. HSTS coverage is inconsistent and no domain in the estate\n  is DNSSEC-signed.\nfindings:\n- lithium.com and www.lithium.com serve an expired TLS certificate (expired 2026-01-03) while asserting\n  HSTS with a one-year max-age — browsers that have seen the header cannot click through.\n- No domain in the estate (khoros.ai, khoros.com, lithium.com, spredfast.com, flow.ai) is DNSSEC-signed.\n- CAA records\
  \ exist only on khoros.com and flow.ai; khoros.ai, lithium.com and spredfast.com publish none.\n- khoros.ai DMARC policy is p=none (monitor only) while khoros.com, lithium.com and spredfast.com are\n  p=reject — the primary brand domain is the weakest of the set.\n- HSTS is absent on every API host except community.khoros.com, including the OAuth authorization server\n  login.spredfast.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/security/lithium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Community
- Social Media
- Customer Engagement
- Customer Support
- Chatbots
- Messaging
- Analytics
- Marketing
---
