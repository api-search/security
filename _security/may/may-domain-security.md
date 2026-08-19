---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:antoine@may.app; pct=90; sp=none
  dnssec: false
  domain: may.app
  mx: Google Workspace
  spf: true
  spf_record: v=spf1 include:_mailcust.gandi.net include:_spf.google.com ~all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=90; sp=none;
  dnssec: false
  domain: may-sante.com
  mx: Google Workspace
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cdn: Cloudflare
  cert_expires: Sep 20 19:55:02 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: www.may.app
  hsts: false
  https: true
  note: Canonical marketing host. Apex may.app 301-redirects here.
  stack: WordPress (Rank Math SEO, WPML, WP Rocket; theme by studiometa)
  tls_version: TLSv1.3
- cdn: Cloudflare
  cert_expires: Sep 19 19:00:26 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: may-sante.com
  hsts: false
  https: true
  note: Legacy brand domain (the URL Serena's portfolio profile lists). Serves a 301 to https://www.may.app/ on both the apex and the www host. No content of its own.
  tls_version: TLSv1.3
- host: capig.may.app
  https: false
  note: 'DANGLING CNAME. Found in certificate-transparency logs. Resolves to k8s-cloudbridgeingres-9547b3803a-310062026.eu-west-3.elb.amazonaws.com, an AWS Kubernetes ingress load balancer in eu-west-3 (Paris) that no longer resolves, so the hostname cannot be reached at all (curl: could not resolve host). It is the only trace of an application backend anywhere in May''s public DNS, and it is decommissioned. A dangling CNAME to a deleted ELB is worth the company''s attention as a subdomain-takeover surface, but it is not an API surface.'
- host: go.may.app
  https: false
  note: Present in certificate-transparency logs but does not resolve in DNS. Almost certainly a retired link-shortener/deep-link host (the site's app-download buttons now point at app.adjust.com).
kind: domain-security
layout: security
method: probed
name: May Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for May, probed live across 4 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: May
provider_slug: may
slug: may-domain-security
source_filename: may-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + certificate-transparency subdomains\nnote: >-\n  May publishes no API, so there is no baseURL and no OpenAPI servers[] host to probe. The\n  hosts below are the canonical marketing host, the legacy brand domain that redirects to\n  it, and the two additional subdomains found in certificate-transparency logs (crt.sh) for\n  *.may.app. Everything sits behind Cloudflare. Neither registrable domain serves HSTS,\n  publishes a CAA record, or is DNSSEC-signed; both publish SPF and a DMARC record at\n  p=quarantine with pct=90 and sp=none, so subdomain mail is unprotected and 10% of failing\n  mail on the organizational domain is still delivered unquarantined. Absence of a record\n  here is observed data, not a gap in the probe.\nhosts:\n- host: www.may.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:55:02 2026 GMT\n  cert_issuer: Google Trust Services (WE1)\n  hsts:\
  \ false\n  cdn: Cloudflare\n  stack: WordPress (Rank Math SEO, WPML, WP Rocket; theme by studiometa)\n  note: Canonical marketing host. Apex may.app 301-redirects here.\n- host: may-sante.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:00:26 2026 GMT\n  cert_issuer: Google Trust Services (WE1)\n  hsts: false\n  cdn: Cloudflare\n  note: >-\n    Legacy brand domain (the URL Serena's portfolio profile lists). Serves a 301 to\n    https://www.may.app/ on both the apex and the www host. No content of its own.\n- host: capig.may.app\n  https: false\n  note: >-\n    DANGLING CNAME. Found in certificate-transparency logs. Resolves to\n    k8s-cloudbridgeingres-9547b3803a-310062026.eu-west-3.elb.amazonaws.com, an AWS\n    Kubernetes ingress load balancer in eu-west-3 (Paris) that no longer resolves, so the\n    hostname cannot be reached at all (curl: could not resolve host). It is the only trace\n    of an application backend anywhere in May's public DNS, and it is decommissioned.\
  \ A\n    dangling CNAME to a deleted ELB is worth the company's attention as a subdomain-takeover\n    surface, but it is not an API surface.\n- host: go.may.app\n  https: false\n  note: >-\n    Present in certificate-transparency logs but does not resolve in DNS. Almost certainly a\n    retired link-shortener/deep-link host (the site's app-download buttons now point at\n    app.adjust.com).\ndomains:\n- domain: may.app\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_mailcust.gandi.net include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:antoine@may.app; pct=90; sp=none\n  mx: Google Workspace\n- domain: may-sante.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; pct=90; sp=none;\n  mx: Google Workspace\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/may/refs/heads/main/security/may-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Digital Health
- Parenting
- Pregnancy
- Maternal Health
- Consumer Health
- Mobile Application
- Employee Benefits
- France
---
