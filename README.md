# ITI.DSGj

The html pages can be viewed as [published by github pages here](https://ihe.github.io/ITI.DSGj/). Note that this does not include the CSS that will be used for formal publication in the Technical framework.

DSG with JSON signature

- Volume 1 changes to [1:37 Document Digital Signature (DSG)](ch-37.html)
- Volume 3 add [3:5.10 Document Digital Signature (DSG) JSON Signature Document Content](ch-5.10.html)
- May update the xml-signature, but those likely will go into CPs to track, see below for the [issues identified in XML DSG chapter 5.5](#issues-identified-in-xml-dsg-chapter-55)

## Zulip Chat

Discussion on [zulip chat stream: IHE DSG using JSON signature](https://chat.fhir.org/#narrow/stream/179223-ihe/topic/IHE-DSG.20using.20JSON.20Signature)

## Working TCON

Weekly on Wednesday until May 10, 2024, at 7am Central, 
[IHE ITI Teams meeting](https://teams.microsoft.com/l/meetup-join/19%3ameeting_MDk4ZDc2MjEtZGZjNy00MzY4LTg2NTgtOTc0ZWQ4YTg5Mjlm%40thread.v2/0?context=%7b%22Tid%22%3a%2202a9376b-a4f9-4a63-a240-52c43ebf9a89%22%2c%22Oid%22%3a%226459fea4-110a-4d17-85f0-00587211a0c0%22%7d)

## Open Issues

#### 1. [Notes about deviation from profile are not being stated in the DSGj profile.](https://github.com/IHE/ITI.DSGj/issues/13)

#### 2. [The usage of DSGj with MHD(ITI-105) is not covered by the DSGj chapter.](https://github.com/IHE/ITI.DSGj/issues/14)

#### 3. [DSGj does not contain guidance around homeCommunityID](https://github.com/IHE/ITI.DSGj/issues/15)

## Issues Identified in XML DSG chapter 5.5

#### 1. Notes about deviation from profile to be reviewed if they need to be present

#### 2. The requirement of "Shall use the canonicalization algorithm “Canonical XML 1.1 with Comments” ( http://www.w3.org/2006/12/xml-c14n11#WithComments )." needs to be reviewed
 <span>The JADES specification is proposing that the signature is applied across a byte stream and makes no assumptions about the canonicalization applied and that canonicalization recommendations are made consistent by PCC dev1</span>

#### 3. Table 5.5.2-1: Digital Signature Purposes from ASTM E1762-95(2013) to be replaced by FHIR Signature Type Value Set

#### 4. Rename the volume 3 to include XML-Signature

#### 5. There is no guidance on encryption algorithms in the chapter at the moment. Review 5.10.2.1.1. "Alg" parameter guidance around "RS256", "ES256" to see if XML needs similar updates