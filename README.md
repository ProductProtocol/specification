# Product Protocol Specification
A protocol specification for crowdfunding/crowdlending campaigns based on digital assets issuing, integration with all business processes, funds management and financial operations.

Protocol describes all milestones and campaign parameters.


## Introduction

There are several problems in ICO/crowdfunding campaigns regarding to:

  1. Low level of business analytics/scoring
  1. Absense of insurance
  1. Low liquidity of issued assets
  1. Unproductive business execution 
  1. Absense of risks management for investors

This standard describes the some way of business developing based on blockchain using it as a tool for transparent processes. 

# Counterparties

  1. Local communication platform (Platform)
  1. Business (Business)
  1. Scoring/analytics and risks management agent (Agent)
  1. Liquidity providers (Market Maker)
  1. Business execution tracker (Tracker)
  1. Insuranse agent (Insurer)


## Platform

Platform is an agent that does the management execution ragarding to all the legal stuff based on it's location and location of all the counterparties are engaged through the whole investing process.


## Business

Business may be present as a launched business or as a business-concept with go-to-market strategy. Platform should make a scoring using some scoring Agent which has a decent expertise in target Business.


## Agent

Agent takes all the risks of money spending for Business. It may use some escrow services to manage the business developmet milestones.


## Market Maker

The goal - is to form some liquidity management strategy, especially for the connected exchanges and market places, minimizes business cash gap consequences.


## Tracker

Tracker can be presented as some foundation with analytics resources.


## Insurer

Some kind of a company which does the communication between the business and investors. Using some business resources it may sign contracts with all the parties in investing process.


# Protocol Parameters

  1. `PLATFORM_ID` - Platform identity
  1. `BUSINESS_ID` - Business legal identity (eg. `Coca-Cola LTD`)
  1. `BUSINESS_LEGAL_HASHSUM` - Business legal verification docs `SHA-256` hashsum (eg. `9913F9B1F619B4116D55C6626F751CBDE7FFBA345849010E6C4B95F6AFB4A606`)
  1. `BUSINESS_LEGAL_EXPIRATION` - Business legal verification expiration `iso8601` date and time (eg. `2019-04-10T14:48:00.000Z`)
  1. `AGENT_ID` - Agent identity
  1. `AGENT_LEGAL_HASHSUM` - Agent legal verification docs `SHA-256` hashsum
  1. `AGENT_LEGAL_EXPIRATION` - Agent legal verification docs expiration date and time
  1. `MARKET_MAKER_ID` - Market Maker identity
  1. `MARKET_MAKER_LEGAL_HASHSUM` - Market Maker legal verification docs `SHA-256` hashsum
  1. `MARKET_MAKER_LEGAL_EXPIRATION` - Market Maker legal verification docs expiration date and time
  1. `TRACKER_ID` - Tracker identity
  1. `TRACKER_LEGAL_HASHSUM` - Tracker legal verification docs
  1. `TRACKER_LEGAL_EXPIRATION` - Tracker legal verification docs expiration date and time
  1. `INSURER_ID` - Insurer identity
  1. `INSURER_LEGAL_HASHSUM` - Insurer legal verification docs
  1. `INSURER_LEGAL_EXPIRATION` - Insurer legal verification docs expiration date and time
  1. `CAMPAIGN_START` - Campaign start date and time
  1. `CAMPAIGN_FINISH` - Campaign finish date and time
  1. `TOKEN_PRICE(DATE_TIME) -> FLOATING POINT` - Lambda function for the virtual asset price
  1. `INVESTOR_ID` - Investor identity
  1. `KYC_PASSED(INVESTOR_ID) -> BOOL` - KYC passing
  1. `ALLOWED_REFUND(DATE_TIME, INVESTOR_ID) -> BOOL` - Lambda refund function


# ACL (Access Control List)

  1. Legal verification docs are unavailable for public access