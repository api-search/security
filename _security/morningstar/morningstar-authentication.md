---
api_key_in: []
api_specs:
- filename: morningstar-oauth-api-openapi.yml
  format: yaml
  label: Morningstar Authentication API
  slug: morningstar-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-oauth-api-openapi.yml
- filename: morningstar-corporate-actions-api-openapi.yml
  format: yaml
  label: Morningstar Time Series API
  slug: morningstar-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-corporate-actions-api-openapi.yml
- filename: morningstar-data-points-api-openapi.yml
  format: yaml
  label: Morningstar Screener APIs
  slug: morningstar-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-data-points-api-openapi.yml
- filename: morningstar-aggregates-financials-api-openapi.yml
  format: yaml
  label: Morningstar Investment Details APIs
  slug: morningstar-investment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-aggregates-financials-api-openapi.yml
- filename: morningstar-investment-list-api-openapi.yml
  format: yaml
  label: Morningstar Investment List API
  slug: morningstar-investment-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-investment-list-api-openapi.yml
- filename: morningstar-esg-api-openapi.yml
  format: yaml
  label: Morningstar Portfolio Analysis APIs
  slug: morningstar-portfolio-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-esg-api-openapi.yml
- filename: morningstar-analyst-highlights-api-openapi.yml
  format: yaml
  label: Morningstar AI Insights API
  slug: morningstar-ai-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-analyst-highlights-api-openapi.yml
- filename: morningstar-scenario-analysis-api-openapi.yml
  format: yaml
  label: Morningstar Scenario Analysis API
  slug: morningstar-scenario-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-scenario-analysis-api-openapi.yml
- filename: morningstar-clients-api-openapi.yml
  format: yaml
  label: Morningstar Risk Profiler API
  slug: morningstar-risk-profiler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-clients-api-openapi.yml
- filename: morningstar-investments-universe-api-openapi.yml
  format: yaml
  label: Morningstar Universe API
  slug: morningstar-universe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-investments-universe-api-openapi.yml
- filename: morningstar-benchmarkfees-api-openapi.yml
  format: yaml
  label: Morningstar Financial Planning APIs
  slug: morningstar-financial-planning-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-benchmarkfees-api-openapi.yml
- filename: morningstar-attribution-api-openapi.yml
  format: yaml
  label: Morningstar Investment Analysis APIs
  slug: morningstar-investment-analysis-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-attribution-api-openapi.yml
- filename: morningstar-accounts-api-openapi.yml
  format: yaml
  label: Morningstar ByAllAccounts API
  slug: morningstar-byallaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-accounts-api-openapi.yml
- filename: morningstar-morningstar-agent-api-openapi.yml
  format: yaml
  label: Morningstar Agent API
  slug: morningstar-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-morningstar-agent-api-openapi.yml
auth_types:
- http-basic (token issuance)
- bearer (API calls)
- oauth2 (MCP server)
description: ''
kind: authentication
layout: security
method: searched
name: Morningstar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode (MCP server only)
overview: Morningstar secures its APIs with http-basic (token issuance), bearer (API calls), and oauth2 (MCP server) across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode (MCP server only) flow(s).
provider_name: Morningstar
provider_slug: morningstar
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/morningstar-accounts-api-openapi.yml
  - openapi/morningstar-activities-api-openapi.yml
  - openapi/morningstar-aggregates-financials-api-openapi.yml
  - openapi/morningstar-aggregates-market-capitalization-and-enterprise-value-api-openapi.yml
  - openapi/morningstar-aggregates-residual-risk-and-return-sensitivity-api-openapi.yml
  - openapi/morningstar-aggregates-returns-api-openapi.yml
  - openapi/morningstar-analyst-highlights-api-openapi.yml
  - openapi/morningstar-analyst-normalized-financials-api-openapi.yml
  - openapi/morningstar-attribution-api-openapi.yml
  - openapi/morningstar-autocomplete-api-openapi.yml
  - openapi/morningstar-basic-details-api-openapi.yml
  - openapi/morningstar-basic-reference-api-openapi.yml
  - openapi/morningstar-benchmarkfees-api-openapi.yml
  - openapi/morningstar-buckets-api-openapi.yml
  - openapi/morningstar-clients-api-openapi.yml
  - openapi/morningstar-company-entitlements-api-openapi.yml
  - openapi/morningstar-compensation-api-openapi.yml
  - openapi/morningstar-consensus-estimates-api-openapi.yml
  - openapi/morningstar-consensus-recommendations-api-openapi.yml
  - openapi/morningstar-corporate-actions-api-openapi.yml
  - openapi/morningstar-corporate-actions-price-mergers-and-acquisitions-api-openapi.yml
  - openapi/morningstar-credentials-api-openapi.yml
  - openapi/morningstar-cusip-api-openapi.yml
  - openapi/morningstar-cusip-change-api-openapi.yml
  - openapi/morningstar-custodians-api-openapi.yml
  - openapi/morningstar-data-points-api-openapi.yml
  - openapi/morningstar-decomposition-api-openapi.yml
  - openapi/morningstar-earnings-summaries-api-openapi.yml
  - openapi/morningstar-equity-company-research-api-openapi.yml
  - openapi/morningstar-equity-moat-framework-api-openapi.yml
  - openapi/morningstar-equity-reports-quant-and-enhanced-quant-api-openapi.yml
  - openapi/morningstar-equity-rps-document-api-openapi.yml
  - openapi/morningstar-esg-api-openapi.yml
  - openapi/morningstar-exposures-api-openapi.yml
  - openapi/morningstar-fees-expenses-api-openapi.yml
  - openapi/morningstar-financials-api-openapi.yml
  - openapi/morningstar-flow-attribution-api-openapi.yml
  - openapi/morningstar-fund-level-sustainability-ratings-research-and-analytics-api-openapi.yml
  - openapi/morningstar-fund-reports-carbon-report-api-openapi.yml
  - openapi/morningstar-fund-reports-esg-api-openapi.yml
  - openapi/morningstar-fund-reports-managed-investment-report-api-openapi.yml
  - openapi/morningstar-fund-reports-target-date-series-api-openapi.yml
  - openapi/morningstar-fund-research-ratings-and-analytics-api-openapi.yml
  - openapi/morningstar-governance-api-openapi.yml
  - openapi/morningstar-holdings-api-openapi.yml
  - openapi/morningstar-households-api-openapi.yml
  - openapi/morningstar-hypo-api-openapi.yml
  - openapi/morningstar-hypothetical-performance-api-openapi.yml
  - openapi/morningstar-idr-investment-details-report-api-openapi.yml
  - openapi/morningstar-industry-classification-api-openapi.yml
  - openapi/morningstar-industry-specific-metrics-api-openapi.yml
  - openapi/morningstar-investment-details-api-openapi.yml
  - openapi/morningstar-investment-list-api-openapi.yml
  - openapi/morningstar-investment-profiles-api-openapi.yml
  - openapi/morningstar-investments-universe-api-openapi.yml
  - openapi/morningstar-key-events-api-openapi.yml
  - openapi/morningstar-macro-shock-scenarios-api-openapi.yml
  - openapi/morningstar-market-capitalization-and-enterprise-value-api-openapi.yml
  - openapi/morningstar-market-shock-scenarios-api-openapi.yml
  - openapi/morningstar-models-api-openapi.yml
  - openapi/morningstar-morningstar-agent-api-openapi.yml
  - openapi/morningstar-oauth-api-openapi.yml
  - openapi/morningstar-office-client-api-openapi.yml
  - openapi/morningstar-office-institution-client-api-openapi.yml
  - openapi/morningstar-office-members-api-openapi.yml
  - openapi/morningstar-ownership-asset-managers-api-openapi.yml
  - openapi/morningstar-ownership-insiders-api-openapi.yml
  - openapi/morningstar-ownership-managed-investments-api-openapi.yml
  - openapi/morningstar-ownership-regulatory-reporting-api-openapi.yml
  - openapi/morningstar-ownership-summary-api-openapi.yml
  - openapi/morningstar-performance-api-openapi.yml
  - openapi/morningstar-persons-api-openapi.yml
  - openapi/morningstar-pjm-professional-judgement-matrix-api-openapi.yml
  - openapi/morningstar-plan-api-openapi.yml
  - openapi/morningstar-plannames-api-openapi.yml
  - openapi/morningstar-portfolio-analytics-api-openapi.yml
  - openapi/morningstar-portfolio-holdings-api-openapi.yml
  - openapi/morningstar-portfolio-holdings-dates-api-openapi.yml
  - openapi/morningstar-portfolio-risk-score-api-openapi.yml
  - openapi/morningstar-portfoliooptimizer-api-openapi.yml
  - openapi/morningstar-portfolios-api-openapi.yml
  - openapi/morningstar-positions-api-openapi.yml
  - openapi/morningstar-professional-judgement-matrices-api-openapi.yml
  - openapi/morningstar-profiles-api-openapi.yml
  - openapi/morningstar-quantitative-comparables-api-openapi.yml
  - openapi/morningstar-quantitative-equity-rating-analysis-api-openapi.yml
  - openapi/morningstar-quantitative-equity-research-ratings-api-openapi.yml
  - openapi/morningstar-questionnaires-api-openapi.yml
  - openapi/morningstar-reference-api-openapi.yml
  - openapi/morningstar-reference-change-api-openapi.yml
  - openapi/morningstar-report-files-api-openapi.yml
  - openapi/morningstar-reports-api-openapi.yml
  - openapi/morningstar-research-ratings-most-recent-and-historical-api-openapi.yml
  - openapi/morningstar-research-ratings-most-recent-api-openapi.yml
  - openapi/morningstar-residual-risk-and-return-sensitivity-api-openapi.yml
  - openapi/morningstar-returns-api-openapi.yml
  - openapi/morningstar-risk-scores-api-openapi.yml
  - openapi/morningstar-scenario-analysis-api-openapi.yml
  - openapi/morningstar-screener-api-openapi.yml
  - openapi/morningstar-securities-api-openapi.yml
  - openapi/morningstar-sedol-api-openapi.yml
  - openapi/morningstar-sedol-change-api-openapi.yml
  - openapi/morningstar-sensitivity-analysis-api-openapi.yml
  - openapi/morningstar-shareholder-stewardship-api-openapi.yml
  - openapi/morningstar-short-interest-api-openapi.yml
  - openapi/morningstar-solutions-api-openapi.yml
  - openapi/morningstar-statement-details-api-openapi.yml
  - openapi/morningstar-statistics-api-openapi.yml
  - openapi/morningstar-style-box-api-openapi.yml
  - openapi/morningstar-time-series-api-openapi.yml
  - openapi/morningstar-timeseries-api-openapi.yml
  - openapi/morningstar-token-api-openapi.yml
  - openapi/morningstar-total-shares-outstanding-api-openapi.yml
  - openapi/morningstar-transcripts-api-openapi.yml
  - openapi/morningstar-views-api-openapi.yml
  - openapi/morningstar-x-ray-api-openapi.yml
  - openapi/morningstar-x-rays-api-openapi.yml
  type: http
slug: morningstar-authentication
source_filename: morningstar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/morningstar-accounts-api-openapi.yml, openapi/morningstar-activities-api-openapi.yml,\n  openapi/morningstar-aggregates-financials-api-openapi.yml, openapi/morningstar-aggregates-market-capitalization-and-enterprise-value-api-openapi.yml,\n  openapi/morningstar-aggregates-residual-risk-and-return-sensitivity-api-openapi.yml, openapi/morningstar-aggregates-returns-api-openapi.yml,\n  openapi/morningstar-analyst-highlights-api-openapi.yml, openapi/morningstar-analyst-normalized-financials-api-openapi.yml,\n  openapi/morningstar-attribution-api-openapi.yml, openapi/morningstar-autocomplete-api-openapi.yml, openapi/morningstar-basic-details-api-openapi.yml,\n  openapi/morningstar-basic-reference-api-openapi.yml ...\nsummary:\n  types:\n  - http-basic (token issuance)\n  - bearer (API calls)\n  - oauth2 (MCP server)\n  oauth2_flows:\n  - authorizationCode (MCP server only)\nschemes:\n- name: BasicAuth\n  type: http\n  scheme:\
  \ basic\n  sources:\n  - openapi/morningstar-accounts-api-openapi.yml\n  - openapi/morningstar-activities-api-openapi.yml\n  - openapi/morningstar-aggregates-financials-api-openapi.yml\n  - openapi/morningstar-aggregates-market-capitalization-and-enterprise-value-api-openapi.yml\n  - openapi/morningstar-aggregates-residual-risk-and-return-sensitivity-api-openapi.yml\n  - openapi/morningstar-aggregates-returns-api-openapi.yml\n  - openapi/morningstar-analyst-highlights-api-openapi.yml\n  - openapi/morningstar-analyst-normalized-financials-api-openapi.yml\n  - openapi/morningstar-attribution-api-openapi.yml\n  - openapi/morningstar-autocomplete-api-openapi.yml\n  - openapi/morningstar-basic-details-api-openapi.yml\n  - openapi/morningstar-basic-reference-api-openapi.yml\n  - openapi/morningstar-benchmarkfees-api-openapi.yml\n  - openapi/morningstar-buckets-api-openapi.yml\n  - openapi/morningstar-clients-api-openapi.yml\n  - openapi/morningstar-company-entitlements-api-openapi.yml\n  - openapi/morningstar-compensation-api-openapi.yml\n\
  \  - openapi/morningstar-consensus-estimates-api-openapi.yml\n  - openapi/morningstar-consensus-recommendations-api-openapi.yml\n  - openapi/morningstar-corporate-actions-api-openapi.yml\n  - openapi/morningstar-corporate-actions-price-mergers-and-acquisitions-api-openapi.yml\n  - openapi/morningstar-credentials-api-openapi.yml\n  - openapi/morningstar-cusip-api-openapi.yml\n  - openapi/morningstar-cusip-change-api-openapi.yml\n  - openapi/morningstar-custodians-api-openapi.yml\n  - openapi/morningstar-data-points-api-openapi.yml\n  - openapi/morningstar-decomposition-api-openapi.yml\n  - openapi/morningstar-earnings-summaries-api-openapi.yml\n  - openapi/morningstar-equity-company-research-api-openapi.yml\n  - openapi/morningstar-equity-moat-framework-api-openapi.yml\n  - openapi/morningstar-equity-reports-quant-and-enhanced-quant-api-openapi.yml\n  - openapi/morningstar-equity-rps-document-api-openapi.yml\n  - openapi/morningstar-esg-api-openapi.yml\n  - openapi/morningstar-exposures-api-openapi.yml\n\
  \  - openapi/morningstar-fees-expenses-api-openapi.yml\n  - openapi/morningstar-financials-api-openapi.yml\n  - openapi/morningstar-flow-attribution-api-openapi.yml\n  - openapi/morningstar-fund-level-sustainability-ratings-research-and-analytics-api-openapi.yml\n  - openapi/morningstar-fund-reports-carbon-report-api-openapi.yml\n  - openapi/morningstar-fund-reports-esg-api-openapi.yml\n  - openapi/morningstar-fund-reports-managed-investment-report-api-openapi.yml\n  - openapi/morningstar-fund-reports-target-date-series-api-openapi.yml\n  - openapi/morningstar-fund-research-ratings-and-analytics-api-openapi.yml\n  - openapi/morningstar-governance-api-openapi.yml\n  - openapi/morningstar-holdings-api-openapi.yml\n  - openapi/morningstar-households-api-openapi.yml\n  - openapi/morningstar-hypo-api-openapi.yml\n  - openapi/morningstar-hypothetical-performance-api-openapi.yml\n  - openapi/morningstar-idr-investment-details-report-api-openapi.yml\n  - openapi/morningstar-industry-classification-api-openapi.yml\n\
  \  - openapi/morningstar-industry-specific-metrics-api-openapi.yml\n  - openapi/morningstar-investment-details-api-openapi.yml\n  - openapi/morningstar-investment-list-api-openapi.yml\n  - openapi/morningstar-investment-profiles-api-openapi.yml\n  - openapi/morningstar-investments-universe-api-openapi.yml\n  - openapi/morningstar-key-events-api-openapi.yml\n  - openapi/morningstar-macro-shock-scenarios-api-openapi.yml\n  - openapi/morningstar-market-capitalization-and-enterprise-value-api-openapi.yml\n  - openapi/morningstar-market-shock-scenarios-api-openapi.yml\n  - openapi/morningstar-models-api-openapi.yml\n  - openapi/morningstar-morningstar-agent-api-openapi.yml\n  - openapi/morningstar-oauth-api-openapi.yml\n  - openapi/morningstar-office-client-api-openapi.yml\n  - openapi/morningstar-office-institution-client-api-openapi.yml\n  - openapi/morningstar-office-members-api-openapi.yml\n  - openapi/morningstar-ownership-asset-managers-api-openapi.yml\n  - openapi/morningstar-ownership-insiders-api-openapi.yml\n\
  \  - openapi/morningstar-ownership-managed-investments-api-openapi.yml\n  - openapi/morningstar-ownership-regulatory-reporting-api-openapi.yml\n  - openapi/morningstar-ownership-summary-api-openapi.yml\n  - openapi/morningstar-performance-api-openapi.yml\n  - openapi/morningstar-persons-api-openapi.yml\n  - openapi/morningstar-pjm-professional-judgement-matrix-api-openapi.yml\n  - openapi/morningstar-plan-api-openapi.yml\n  - openapi/morningstar-plannames-api-openapi.yml\n  - openapi/morningstar-portfolio-analytics-api-openapi.yml\n  - openapi/morningstar-portfolio-holdings-api-openapi.yml\n  - openapi/morningstar-portfolio-holdings-dates-api-openapi.yml\n  - openapi/morningstar-portfolio-risk-score-api-openapi.yml\n  - openapi/morningstar-portfoliooptimizer-api-openapi.yml\n  - openapi/morningstar-portfolios-api-openapi.yml\n  - openapi/morningstar-positions-api-openapi.yml\n  - openapi/morningstar-professional-judgement-matrices-api-openapi.yml\n  - openapi/morningstar-profiles-api-openapi.yml\n\
  \  - openapi/morningstar-quantitative-comparables-api-openapi.yml\n  - openapi/morningstar-quantitative-equity-rating-analysis-api-openapi.yml\n  - openapi/morningstar-quantitative-equity-research-ratings-api-openapi.yml\n  - openapi/morningstar-questionnaires-api-openapi.yml\n  - openapi/morningstar-reference-api-openapi.yml\n  - openapi/morningstar-reference-change-api-openapi.yml\n  - openapi/morningstar-report-files-api-openapi.yml\n  - openapi/morningstar-reports-api-openapi.yml\n  - openapi/morningstar-research-ratings-most-recent-and-historical-api-openapi.yml\n  - openapi/morningstar-research-ratings-most-recent-api-openapi.yml\n  - openapi/morningstar-residual-risk-and-return-sensitivity-api-openapi.yml\n  - openapi/morningstar-returns-api-openapi.yml\n  - openapi/morningstar-risk-scores-api-openapi.yml\n  - openapi/morningstar-scenario-analysis-api-openapi.yml\n  - openapi/morningstar-screener-api-openapi.yml\n  - openapi/morningstar-securities-api-openapi.yml\n  - openapi/morningstar-sedol-api-openapi.yml\n\
  \  - openapi/morningstar-sedol-change-api-openapi.yml\n  - openapi/morningstar-sensitivity-analysis-api-openapi.yml\n  - openapi/morningstar-shareholder-stewardship-api-openapi.yml\n  - openapi/morningstar-short-interest-api-openapi.yml\n  - openapi/morningstar-solutions-api-openapi.yml\n  - openapi/morningstar-statement-details-api-openapi.yml\n  - openapi/morningstar-statistics-api-openapi.yml\n  - openapi/morningstar-style-box-api-openapi.yml\n  - openapi/morningstar-time-series-api-openapi.yml\n  - openapi/morningstar-timeseries-api-openapi.yml\n  - openapi/morningstar-token-api-openapi.yml\n  - openapi/morningstar-total-shares-outstanding-api-openapi.yml\n  - openapi/morningstar-transcripts-api-openapi.yml\n  - openapi/morningstar-views-api-openapi.yml\n  - openapi/morningstar-x-ray-api-openapi.yml\n  - openapi/morningstar-x-rays-api-openapi.yml\ndocs: https://developer.morningstar.com/direct-web-services/documentation/api-utilities/authentication-api/overview\ndetails:\n  token_issuance:\
  \ POST /token/oauth on the regional base (us/emea/apac-api.morningstar.com) with Basic\n    Base64 username:password returns an unscoped bearer access token.\n  token_ttl_minutes: 60\n  token_cache_note: Requests within ten minutes of issuance return the same cached token.\n  credential_provisioning: Sales-gated - usernames/passwords are provisioned during Morningstar onboarding;\n    no self-serve signup.\n  market_data_note: Market Data Web Services uses IP-allowlisted username/password on client-specific\n    servers.\n  mcp_oauth: The MCP server at mcp.morningstar.com runs a full OAuth 2.0 authorization server with PKCE\n    (S256) and dynamic client registration - see well-known/morningstar-oauth-authorization-server.json\n    and scopes/morningstar-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/authentication/morningstar-authentication.yml
summary_line: http-basic (token issuance)/bearer (API calls)/oauth2 (MCP server) · 1 scheme
tags:
- Financial
- Market Data
- Investing
- Stocks
- Funds
- Real-Time
- Reference Data
- Portfolio Analytics
- Research
- Indexes
---
