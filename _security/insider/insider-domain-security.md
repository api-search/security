---
api_specs:
- filename: insider-unification-openapi.yml
  format: yaml
  label: Insider One Unification API
  slug: insider-one-unification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-unification-openapi.yml
- filename: insider-contact-openapi.yml
  format: yaml
  label: Insider One Contact API
  slug: insider-one-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-contact-openapi.yml
- filename: insider-mail-openapi.yml
  format: yaml
  label: Insider One Mail API
  slug: insider-one-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mail-openapi.yml
- filename: insider-sms-openapi.yml
  format: yaml
  label: Insider One SMS API
  slug: insider-one-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-sms-openapi.yml
- filename: insider-whatsapp-openapi.yml
  format: yaml
  label: Insider One WhatsApp API
  slug: insider-one-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-whatsapp-openapi.yml
- filename: insider-gateway-openapi.yml
  format: yaml
  label: Insider One Gateway API (OAuth 2.0)
  slug: insider-one-gateway-api-oauth-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-gateway-openapi.yml
- filename: insider-web-push-openapi.yml
  format: yaml
  label: Insider One Web Push API
  slug: insider-one-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-web-push-openapi.yml
- filename: insider-mobile-openapi.yml
  format: yaml
  label: Insider One Mobile App API
  slug: insider-one-mobile-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mobile-openapi.yml
- filename: insider-mobile-settings-openapi.yml
  format: yaml
  label: Insider One Mobile Settings API
  slug: insider-one-mobile-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mobile-settings-openapi.yml
- filename: insider-live-activity-openapi.yml
  format: yaml
  label: Insider One Live Activity API
  slug: insider-one-live-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-live-activity-openapi.yml
- filename: insider-verify-openapi.yml
  format: yaml
  label: Insider One Verify (OTP) API
  slug: insider-one-verify-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-verify-openapi.yml
- filename: insider-catalog-openapi.yml
  format: yaml
  label: Insider One Catalog API
  slug: insider-one-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-catalog-openapi.yml
- filename: insider-recommendation-openapi.yml
  format: yaml
  label: Insider One Recommendation API
  slug: insider-one-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-recommendation-openapi.yml
- filename: insider-eureka-search-openapi.yml
  format: yaml
  label: Insider One Eureka Search API
  slug: insider-one-eureka-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-eureka-search-openapi.yml
- filename: insider-eureka-events-openapi.yml
  format: yaml
  label: Insider One Eureka Event Collection API
  slug: insider-one-eureka-event-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-eureka-events-openapi.yml
- filename: insider-analytics-openapi.yml
  format: yaml
  label: Insider One Analytics API
  slug: insider-one-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-analytics-openapi.yml
- filename: insider-architect-analytics-openapi.yml
  format: yaml
  label: Insider One Architect Analytics API
  slug: insider-one-architect-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-architect-analytics-openapi.yml
- filename: insider-architect-transactional-openapi.yml
  format: yaml
  label: Insider One Architect Transactional Journey API
  slug: insider-one-architect-transactional-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-architect-transactional-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: insiderone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: useinsider.com
  spf: true
hosts:
- cert_expires: Nov  4 12:40:39 2026 GMT
  host: insiderone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 02:45:57 2026 GMT
  host: academy.insiderone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 03:30:39 2026 GMT
  host: unification.useinsider.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insider Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insider, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Insider
provider_slug: insider
slug: insider-domain-security
source_filename: insider-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insiderone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 12:40:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: academy.insiderone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 02:45:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: unification.useinsider.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:30:39 2026 GMT\n  hsts: null\ndomains:\n- domain: insiderone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: useinsider.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/security/insider-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Customer Engagement
- Personalization
- Customer Data Platform
- Marketing
- Journey Orchestration
- Omnichannel
- CDP
- Artificial Intelligence
- Messaging
- WhatsApp
- Email
- SMS
- Push Notifications
- Recommendations
- Search
- Product Catalog
- Analytics
- MCP
- Agents
- Consent
- GDPR
---
