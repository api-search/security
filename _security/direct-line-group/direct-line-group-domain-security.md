---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: directline.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: churchill.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greenflag.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: privilege.com
  note: The only group domain with a permissive DMARC policy (p=none — monitor only).
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: mailto:dmarcadmin@darwin-insurance.com
  dnssec: false
  domain: darwin-insurance.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: darwin.co.uk
  in_group: false
  note: Not a group domain — GoDaddy aftermarket listing. Excluded from the summary counts below.
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bymiles.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: directlineforbusiness.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: directlinegroup.co.uk
  spf: true
hosts:
- cert_expires: Jan 25 12:49:05 2027 GMT
  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=www.directline.com
  host: www.directline.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 12:49:05 2027 GMT
  host: www.churchill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 09:54:18 2027 GMT
  host: www.greenflag.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 12:49:05 2027 GMT
  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=www.directline.com
  host: www.privilege.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Serves the shared www.directline.com certificate — the Privilege brand site runs on the same UK Insurance Limited web estate.
  tls_version: TLSv1.3
- cert_expires: Jan 30 11:13:55 2027 GMT
  cert_subject: CN=www.darwin-insurance.com
  host: www.darwin-insurance.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: The real Darwin brand site. Policies underwritten by U K Insurance Limited (the Direct Line Group entity, FCA No. 536726) and arranged/administered by iGO4 Limited.
  tls_version: TLSv1.3
- cert_expires: Aug  2 18:53:30 2026 GMT
  cert_subject: CN=www.darwin.co.uk
  host: www.darwin.co.uk
  hsts: false
  https: true
  in_group: false
  note: NOT a Direct Line Group property. Probed and excluded 2026-07-25 — the host serves a one-line HTML redirector to /lander, which forwards to forsale.godaddy.com/forsale/www.darwin.co.uk, and its /llms.txt states the domain is listed for sale on GoDaddy's aftermarket. Retained here only to record the exclusion so a later round does not re-adopt it.
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  cert_subject: CN=bymiles.co.uk
  host: www.bymiles.co.uk
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:48:51 2026 GMT
  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=*.directlineforbusiness.co.uk
  host: www.directlineforbusiness.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expired: true
  cert_expires: Jun 15 12:34:59 2026 GMT
  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=api.directlinegroup.co.uk
  host: api.directlinegroup.co.uk
  hsts: null
  http_status: 403
  https: true
  note: MuleSoft Anypoint production load balancer (dlg-production-load-balancer.lb.anypointdns.net). Certificate expired 2026-06-15 and has not been renewed; the server sends a TLS CertificateRequest (mutual TLS) and returns an nginx HTTP 403 at every path probed. Partner/internal gateway, not a developer surface.
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  cert_subject: CN=bymiles.co.uk
  host: api.bymiles.co.uk
  hsts: null
  http_status: 403
  https: true
  note: Amazon API Gateway (response headers x-amz-apigw-id, x-amzn-errortype ForbiddenException). Root returns {"message":"Forbidden"}; /v1/* returns {"message":"Missing Authentication Token"}. Gated, undocumented. Discovered 2026-07-25 by DNS enumeration — not recorded in the 2026-07-25 initial review.
  tls_version: TLSv1.3
- error: 'TLS handshake failed: tlsv1 unrecognized name (no certificate presented for this SNI name)'
  host: api.darwin.co.uk
  https: false
  note: Resolves to AWS anycast addresses (13.248.169.48, 76.223.54.146) but presents no certificate for the name; not a usable public host.
- cert_expires: Sep 28 08:47:41 2026 GMT
  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=docs.directline.com
  host: docs.directline.com
  hsts: null
  http_status: 200
  https: true
  note: Form-based login wall titled "DirectLine - Login"; no reference documentation. Lowest TLS version observed across the estate (TLSv1.2).
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Direct Line Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Direct Line Group, probed live across 12 host(s) and 9 registrable domain(s). 11 host(s) serve HTTPS (up to TLSv1.3); 7 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Direct Line Group
provider_slug: direct-line-group
slug: direct-line-group-domain-security
source_filename: direct-line-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Direct Line Group brand host, the group\n  API host, and the two brand API hosts discovered by DNS enumeration on 2026-07-25\nhosts:\n- host: www.directline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 12:49:05 2027 GMT\n  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=www.directline.com\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.churchill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 12:49:05 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.greenflag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 09:54:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.privilege.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 12:49:05 2027 GMT\n  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=www.directline.com\n  hsts: true\n  hsts_max_age:\
  \ 63072000\n  note: Serves the shared www.directline.com certificate — the Privilege brand site\n    runs on the same UK Insurance Limited web estate.\n- host: www.darwin-insurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 11:13:55 2027 GMT\n  cert_subject: CN=www.darwin-insurance.com\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: The real Darwin brand site. Policies underwritten by U K Insurance Limited\n    (the Direct Line Group entity, FCA No. 536726) and arranged/administered by\n    iGO4 Limited.\n- host: www.darwin.co.uk\n  in_group: false\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 18:53:30 2026 GMT\n  cert_subject: CN=www.darwin.co.uk\n  hsts: false\n  note: NOT a Direct Line Group property. Probed and excluded 2026-07-25 — the host\n    serves a one-line HTML redirector to /lander, which forwards to\n    forsale.godaddy.com/forsale/www.darwin.co.uk, and its /llms.txt states the\n    domain is listed\
  \ for sale on GoDaddy's aftermarket. Retained here only to\n    record the exclusion so a later round does not re-adopt it.\n- host: www.bymiles.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  cert_subject: CN=bymiles.co.uk\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.directlineforbusiness.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:48:51 2026 GMT\n  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=*.directlineforbusiness.co.uk\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.directlinegroup.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jun 15 12:34:59 2026 GMT\n  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=api.directlinegroup.co.uk\n  cert_expired: true\n  hsts: null\n  http_status: 403\n  note: MuleSoft Anypoint production load balancer (dlg-production-load-balancer.lb.anypointdns.net).\n    Certificate expired 2026-06-15 and\
  \ has not been renewed; the server sends a TLS\n    CertificateRequest (mutual TLS) and returns an nginx HTTP 403 at every path\n    probed. Partner/internal gateway, not a developer surface.\n- host: api.bymiles.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  cert_subject: CN=bymiles.co.uk\n  hsts: null\n  http_status: 403\n  note: Amazon API Gateway (response headers x-amz-apigw-id, x-amzn-errortype ForbiddenException).\n    Root returns {\"message\":\"Forbidden\"}; /v1/* returns {\"message\":\"Missing Authentication\n    Token\"}. Gated, undocumented. Discovered 2026-07-25 by DNS enumeration — not\n    recorded in the 2026-07-25 initial review.\n- host: api.darwin.co.uk\n  https: false\n  error: 'TLS handshake failed: tlsv1 unrecognized name (no certificate presented for\n    this SNI name)'\n  note: Resolves to AWS anycast addresses (13.248.169.48, 76.223.54.146) but presents\n    no certificate for the name; not a usable public host.\n- host:\
  \ docs.directline.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 08:47:41 2026 GMT\n  cert_subject: C=GB, ST=Kent, L=Bromley, O=Direct Line Insurance Group Plc, CN=docs.directline.com\n  hsts: null\n  http_status: 200\n  note: Form-based login wall titled \"DirectLine - Login\"; no reference documentation.\n    Lowest TLS version observed across the estate (TLSv1.2).\ndomains:\n- domain: directline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: churchill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: greenflag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: privilege.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: The only group domain with a permissive DMARC policy (p=none — monitor only).\n- domain: darwin-insurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n  dmarc_rua: mailto:dmarcadmin@darwin-insurance.com\n- domain: darwin.co.uk\n  in_group: false\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dmarc_policy: null\n  note: Not a group domain — GoDaddy aftermarket listing. Excluded from the summary\n    counts below.\n- domain: bymiles.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: directlineforbusiness.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: directlinegroup.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nsummary:\n  scope_note: Counts cover Direct Line Group properties only; www.darwin.co.uk and\n    darwin.co.uk are recorded above but excluded because they are not group properties.\n  hosts_probed: 11\n  https_reachable: 10\n  hsts_present: 7\n  domains_probed: 8\n  dnssec: 0\n  caa: 0\n  spf: 8\n  dmarc: 7\n  dmarc_reject: 6\n  findings:\n  - Every group domain publishes\
  \ SPF; none publishes CAA and none is DNSSEC-signed.\n  - privilege.com DMARC is p=none (monitor only) while the rest of the estate is p=reject.\n  - The group API host api.directlinegroup.co.uk has been serving an expired certificate\n    since 2026-06-15 while still demanding a client certificate.\n  - www.privilege.com serves the www.directline.com certificate — the Privilege brand\n    runs on the shared U K Insurance Limited web estate.\n  - docs.directline.com is the only host still on TLSv1.2.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/direct-line-group/refs/heads/main/security/direct-line-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Personal Lines
- Motor Insurance
- Home Insurance
- Carrier
- Roadside Assistance
- Partner Gated
---
