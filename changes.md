# 2019-03-27: update to 1.8 specifications ehealth suisse/MOFH after update of specifications from ehealth suisse/MOFH (A5E1/A5E2 V1.8, CH:ATC V1.2.0 ) and online wave 2 testing

see also [EHS-169](https://gazelle.ihe.net/jira/projects/EHS/queues/issue/EHS-169)

1_09_EPR_PatientModifyConfLevelDoc
* added ADR to ITI-57 and ITI-92 and ITI-18 

1_09b_EPR_PatientModifyConfLevelDoc
* added note in title that XDS Affinity Domain Option is used
* precised sequence diagram in remote community
* added XADR to ITI-57 and ITI-92 and ITI-18 

1_07_EPR_PatientCreateEPR
* Renamed Operator to Policy administrator

1_07b_EPR_PatientOpenEPR
* Renamed Operator to Policy administrator

1_10_EPR_PatientVerifiesAccessLog 
* add Authorization Decision Consumer | X-Service User grouped to Patient Audit Record Repository
* added ADR and XADR sequence with Authorization Decision Provider

1_14_EPR_PatientDeleteEPR
* Renamed Operator to Policy administrator
* SEQ002 resolved, (initial) policies can be deleted 

2_02_EPR_HPGetDocuments1of3
* added Policy Enforcement Point to Document Repository and a note for [CH:ADR] Enforcement of XDS Retrieve Document Set transactions (3.1.12)

2_02_EPR_HPGetDocuments2of3
* added ADR and XADR transaction
* added Policy Enforcement Point to Document Repository and a note for [CH:ADR] Enforcement of XDS Retrieve Document Set transactions (3.1.12)

2_03_EPR_HPGetDocuments3of3
* added Policy Enforcement Point to Document Repository and a note for [CH:ADR] Enforcement of XDS Retrieve Document Set transactions (3.1.12)

2_02b_EPR_PatientGetDocuments1of2
* added Policy Enforcement Point to Document Repository and a note for [CH:ADR] Enforcement of XDS Retrieve Document Set transactions (3.1.12)

2_02b_EPR_PatientGetDocuments2of2
* added Policy Enforcement Point to Document Repository and a note for [CH:ADR] Enforcement of XDS Retrieve Document Set transactions (3.1.12)

2_05_EPR_Patient_XDS-I_XCA-I-1of2
* added Policy Enforcement Point to Document Repository and a note for [CH:ADR] Enforcement of XDS Retrieve Document Set transactions (3.1.12)
* added Policy Enforcement Point to Imaging Document Source and a note for [CH:ADR] Enforcement of XDS-I "Imaging Retrieve" transactions (3.1.13)
* removed WADO-55 (Decision AG TSI from 27.2.2019)

2_05_EPR_Patient_XDS-I_XCA-I-2of2
* added Policy Enforcement Point to Imaging Document Source and a note for [CH:ADR] Enforcement of XDS-I "Imaging Retrieve" transactions (3.1.13)

2_05_EPR_XDS-I-XCA-1of2
* added Policy Enforcement Point to Imaging Document Source and a note for [CH:ADR] Enforcement of XDS-I "Imaging Retrieve" transactions (3.1.13)
* added Policy Enforcement Point to Document Repository and a note for [CH:ADR] Enforcement of XDS Retrieve Document Set transactions (3.1.12)
* removed WADO-55 (Decision AG TSI from 27.2.2019)

2_05_EPR_XDS-I-XCA-2of2
* added Policy Enforcement Point to Imaging Document Source and a note for [CH:ADR] Enforcement of XDS-I "Imaging Retrieve" transactions (3.1.13)

# 2018-12-21: update to 1.6 specifications ehealth suisse/MOFH after update of specifications from ehealth suisse/MOFH (A5E1/A5E2 V1.6, CN:ATC V1.1.0 ) 

general updates:
transactions which are neither IHE, eCH or CH:xxx have now a black colored arrow to differentiate 

1_02_EPR_QueryingGovernmentServices - no changes
Note: [ITI-60] Retrieve Multiple Value Sets will get optional, decided at AT TSI Meeting 12.12.18 but not reflected yet in ordinnace

1_02_EPR_QueryingGovernmentServicesHPD - no changes

1_02_EPR_QueryingGovernmentServicesMPI
renamed to -1_02_EPR_QueryingGovernmentServicesMDI

1_02b_EPR_CommunityInCircleOfTrust - no changes

1_03-1_6_HPD_Usecases - no changes

1_07_EPR_PatientCreateEPR
* grouped actor Patient Identity Source and Patient identifier - Cross-reference Consumer (Feedback from JB)
* introduced policy source for feeding initial patient policies into the policy repository by the policy administrator (see A5E1 2.3.2 A special case is the on-boarding process of a new patient)

1_07b_EPR_PatientOpenEPR
* grouped actor Patient Identity Source and Patient identifier - Cross-reference Consumer (Feedback from JB)

1_08_EPR_PatientModifyAccessRights
* resolved Note **SEQ_001** 
    - optional to query MPI_A-PID from MPI using local ID / UAP-ID in portal (for patient portal UAP-ID can be directly provided)
    - optional to resolve it to the EPR-SPID by querying the community data stores.

1_09_EPR_PatientModifyConfLevelDoc
* resolved Note **SEQ_001** 
    - optional to resolve it to the EPR-SPID by querying the community data stores.
* replaced [ITI-X1] with assigned transaction number: [ITI-92]

1_09b_EPR_PatientModifyConfLevelDoc
* resolved Note **SEQ_001** 
    - optional to resolve it to the EPR-SPID by querying the community data stores.
* replaced [ITI-X1] with assigned transaction number: [ITI-92]

1_10_EPR_PatientVerifiesAccessLog
* resolved Note **SEQ_001** 
* added grouped actors Authorization Client / Resource Server

1_14_EPR_PatientDeleteEPR
* introduced policy administrator extension for CH:XUA
* still open question: **SEQ_002**: PPQ: Can all policies for a patient be deleted with a Delete Policy Request?

1_15_EPR_PatientEPRQuery - no changes
1_16_EPR_PatientEPRInactivate  - no changes
2_01_EPR_ATNA - no changes
2_01_EPR_CT - no changes

2_02_EPR_HPGetDocuments
* removed consolidation of 2_02_EPR_HPGetDocuments1of3, 2_02_EPR_HPGetDocuments2of3,2_02_EPR_HPGetDocuments2of3 diagram is to big

2_02_EPR_HPGetDocuments1of3
* adapted CH:XUA Get X-User Assertions with Healthcare Professional Extension
* removed grouped Authorization Decision Consumer actor from Document Repository
* removed note about policy enforcing in repository (now described in 3.1.12 Enforcement of XDS Retrieve Document Set transactions) and added transactions with ITI-18

2_02_EPR_HPGetDocuments2of3
* adapted CH:XUA Get X-User Assertions with Healthcare Professional Extension
* removed grouped Authorization Decision Consumer actor from Document Repository
* removed note about policy enforcing in repository (now described in 3.1.12 Enforcement of XDS Retrieve Document Set transactions) and added transactions with ITI-18

2_02_EPR_HPGetDocuments3of3
* adapted CH:XUA Get X-User Assertions with Healthcare Professional Extension
* removed grouped Authorization Decision Consumer actor from Document Repository
* removed note about policy enforcing in repository (now described in 3.1.12 Enforcement of XDS Retrieve Document Set transactions) and added transactions with ITI-18

2_02b_EPR_PatientGetDocuments1of2
* adapted CH:XUA Get X-User Assertions with Patient Extension
* removed grouped Authorization Decision Consumer actor from Document Repository
* removed note about policy enforcing in repository (now described in 3.1.12 Enforcement of XDS Retrieve Document Set transactions) and added transactions with ITI-18

2_02b_EPR_PatientGetDocuments2of2
* adapted CH:XUA Get X-User Assertions with Patient Extension
* removed grouped Authorization Decision Consumer actor from Document Repository
* removed note about policy enforcing in repository (now described in 3.1.12 Enforcement of XDS Retrieve Document Set transactions) and added transactions with ITI-18

2_03_EPR_HPStoreDocuments
* adapted CH:XUA Get X-User Assertions with Healthcare Professional Extension

2_03b_EPR_PatientStoreDocuments
* adapted CH:XUA Get X-User Assertions with Patient Extension

2_04_EPR_PatientAssignAccessRights
* adapted CH:XUA Get X-User Assertions with Patient Extension

2_05_EPR_Patient_XDS-I_XCA-I_1of2
* adapted CH:XUA Get X-User Assertions with Patient Extension
* removed grouped Authorization Decision Consumer actor from Document Repository
* removed note about policy enforcing in repository (now described in 3.1.12 Enforcement of XDS Retrieve Document Set transactions) and added transactions with ITI-18
* precised for wado that grouping with [ITI-IUA] is an open issues

2_05_EPR_Patient_XDS-I_XCA-I_2of2
* adapted CH:XUA Get X-User Assertions with Patient Extension

2_05_EPR_XDS-I_XCA-I
* removed, described in 2_05_EPR_XDS-I_XCA-I_1of2 and 2_05_EPR_XDS-I_XCA-I_2of2

2_05_EPR_XDS-I_XCA-I_1of2
* adapted CH:XUA Get X-User Assertions with Healthcare Professional Extension
* precised for wado that grouping with [ITI-IUA] is an open issues

2_05_EPR_XDS-I_XCA-I_2of2
* adapted CH:XUA Get X-User Assertions with Healthcare Professional Extension

2_06_EPR_PatientExportDocuments - no changes

2_06_EPR_PatientImportDocuments - no changes

# 2018-07-05: update of specifications from ehealth suisse/MOFH after update of specifications from ehealth suisse/MOFH (A5E1/A5E2 V1.5)

2_05_EPR_Patient_XDS-I_XCA-I_1of2
2_05_EPR_XDS-I_XCA-I_1of2
* readded [RAD-55] WADO Retrieve (E-Mail from David Moessner 2.7 to EPD Projectathon google group: We were planning to remove RAD-55 WADO Retrieve but after a discussion in the working group technical-semantically interoperability some questions were raised which we have to look at first before making a final decision. So for now the transaction will not be removed.)

# 2018-06-19: update of specifications from ehealth suisse/MOFH
Updated specifications for the next Swiss #EPR #projectathon in Bern September 2018, check [eHealth Suisse Relevant Specification]( https://www.e-health-suisse.ch/gemeinschaften-umsetzung/umsetzung/programmierhilfen/relevante-spezifikationen.html) and [overview](https://www.e-health-suisse.ch/fileadmin/user_upload/Dokumente/2018/E/180220_Grafik_Swiss_Electronic_Patient_Record_v1.4_e.pdf) 

1_02_EPR_QueryingGovernmentServices
* removed Secure Node from Patient Portal, Health Professional Portal (no connected transactions, minor)

1_02_EPR_QueryingGovernmentServicesHPD - no change 

1_02_EPR_QueryingGovernmentServicesMPI - no chane

1_02b_EPR_CommunityInCircleOfTrust
* attribute ComStatus is now shcStatus, Inactive instead of inactive
* transaction is called CH:CIQ

1_03-1_6_HPD_Usecases - no changes

1_07_EPR_PatientCreateEPR
* added note: initializing policies will be supported with a next revision of PPQ (decided in AG TSI, 16th meeting, issue EPD-28)
* changed origin of transaction for triggering policies from Patient Identity Source to Operator (Actor will not be specified by PPQ)

1_07b_EPR_PatientOpenEPR - no changes

1_08_EPR_PatientModifyAccessRights - no change, but depending on resolution of **SEQ_001**

1_09_EPR_PatientModifyConfLevelDoc 
* XUA depending on resolution of **SEQ_001**
* Added actors/transaction from RMU as alternative to XDS MU

1_09b_EPR_PatientModifyConfLevelDoc
* XUA depending on resolution of **SEQ_001**
* Replaced actors/transaction from XCMU with RMU (Update Initiator/Responder instead of XCMU Document Administrator)

1_10_EPR_PatientVerifiesAccessLog
* XUA depending on resolution of **SEQ_001**
* Replace deprecated sequence diagram with new sequence diagrams based on CH:ATC Profile

1_12_EPR_PatientDeleteDocument
* removed deprecated sequence diagram, deletion of document is postponed

1_14_EPR_PatientDeleteEPR
* moved optional deletion task from UPI_Client actor to operator
* **SEQ_002**: PPQ: Can all policies for a patient be deleted with a Delete Policy Request?

1_15_EPR_PatientEPRQuery - no changes

1_16_EPR_PatientEPRInactivate - no chnages

2_01_EPR_ATNA
* removed Audit Record Repository actor

2_01_EPR_CT
* removed Government Services HPD/MDI/CPI clients actors and transaction

2_02_EPR_HPGetDocuments
* see 2_02_EPR_HPGetDocuments1of3, 2_02_EPR_HPGetDocuments2of3, 2_02_EPR_HPGetDocuments3of3

2_02_EPR_HPGetDocuments1of3 - TODO
* [04] CH:XUA Authenticate user response added UAP-ID as response identifier for clarification
* [11] CH:XUA Get-XUser Assertions uses UAP-ID for Request (before EPRS-PID)
* [12] **SEQ_003** A5E1 1.6.2.2 states that a data source is need for UAP-Identifier to GLN for a health professional. How can this transformation be done? 
    * A) If the X-Assertion Provider is directly grouped with the Health Professional Portal (X-Service User) then this would be possible because the health professional portal has the information between UAP-ID and local ID. 
    * B) If the X-Assertion Provider is within the community one possiblity would be to register the UAP-ID of the patient in the HPD as an identifier (by the Health Professional Portal?).
    * C) An independent Data Source?
* HPD Information Consumer, Provider grouping have been added

2_02_EPR_HPGetDocuments2of3 
* see 2_02_EPR_HPGetDocuments1of3

2_02_EPR_HPGetDocuments3of3 
* see 2_02_EPR_HPGetDocuments1of3

2_02b_EPR_PatientGetDocuments1of2
* [04] CH:XUA Authenticate user response added UAP-ID as response identifier for clarification
* [11] CH:XUA Get-XUser Assertions uses UAP-ID for Request (before EPRS-PID)
* [12] **SEQ_001** A5E1 1.6.2.2 states that a data source is need for UAP-Identifier to MPI-ID. How can this transformation be done? 
    * A) If the X-Assertion Provider is directly grouped with the Patient Portal (X-Service User) then this would be possible because the patient portal has the information between UAP-ID and local ID of the patient portal. 
    * B) If the X-Assertion Provider is within the community the only possiblity would be to register the UAP-ID of the patient in the MPI (by the Patient Portal?)
    * C) An independent Data Source? Mapping between UAP-ID and MPI-PID is problematic, since the MPI-PID can change.
* [13-15] The EPR-SPID needs to be returned, the X-Assertion Provider nees to call the MPI with a PIX-Query to resolve the EPRS-PID, this has actually already been done in [06-09]

2_02b_EPR_PatientGetDocuments2of2 
* see 2_02b_EPR_PatientGetDocuments1of2

2_03_EPR_HPStoreDocuments
* see 2_02_EPR_HPGetDocuments

2_03b_EPR_PatientStoreDocuments
* see 2_02b_EPR_PatientGetDocuments1of2

2_04_EPR_PatientAssignAccessRights
* see 2_02b_EPR_PatientGetDocuments1of2

2_05_EPR_Patient_XDS-I_XCA-I_1of2
* removed [RAD-55] WADO Retrieve
* open issue grouping CH:XUA with Imaging Document Source
* see 2_02b_EPR_PatientGetDocuments1of2
* removed maturity level text

2_05_EPR_Patient_XDS-I_XCA-I_2of2
* open issue grouping CH:XUA with Imaging Document Source
* see 2_02b_EPR_PatientGetDocuments1of2
* removed maturity level text

2_05_EPR_XDS-I_XCA-I
* see 2_05_EPR_XDS-I_XCA-I_1of2, 2_05_EPR_XDS-I_XCA-I_2of2

2_05_EPR_XDS-I_XCA-I_1of2
* removed [RAD-55] WADO Retrieve
* open issue grouping CH:XUA with Imaging Document Source
* see 2_02_EPR_HPGetDocuments1of3
* removed maturity level text

2_05_EPR_XDS-I_XCA-I_2of2
* open issue grouping CH:XUA with Imaging Document Source
* see 2_02_EPR_HPGetDocuments1of3
* removed maturity level text

2_06_EPR_PatientExportDocuments - new sequence diagram
* XUA depending on resolution of **SEQ_001**
* export of privacy policies is not covered

2_07_EPR_PatientImportDocuments  - new sequence diagram
* XUA depending on resolution of **SEQ_001**

# 2018-03-05: changes after specification update from ehealth suisse/MOFH
Updated specifications for the next Swiss #EPR #projectathon at The Hague @IHE_Europe, check [google group]( https://groups.google.com/forum/#!topic/epd_projectathon/6tHhL_ztSL8epd_projectathon@googlegroups.com) and [overview](https://www.e-health-suisse.ch/fileadmin/user_upload/Dokumente/2018/E/180220_Grafik_Swiss_Electronic_Patient_Record_v1.4_e.pdf) 

1_02_EPR_QueryingGovernmentServices
* introduction of CH:CPI profile: change actor from Community \nPortal \nIndex to CPI Provider, Value Set Consumer to CPI Consumer and added transactions Community Information Query [CH:CIQ] and Community Information [CH:CIDD] Delta Download
* separated CH:PIDD from ITI-58 in HP
* adjusted sub sequence diagrams 1_02_EPR_QueryingGovernmentServicesHPD and 1_02_EPR_QueryingGovernmentServicesMPI

1_02b_EPR_CommunityInCircleOfTrust
* adjusted actors/transctions to CH:CPI profile

1_08_EPR_PatientModifyAccessRights
* adjusted PPQ actors,transaction (split fromm manager to source/consumer and adjust ppq-1, ppq-2 transactions)

1_09b_EPR_PatientModifyConfLevelDoc
* XCPD needs not to be grouped with XUA [ITI-40] Provide X-User Assertion [EPR-SPID] (decision AG TSI meeting)
* Initiating Gateway should be grouped with X-Service User, not X-Service Provider

1_10_EPR_PatientVerifiesAccessLog.plantuml !DEPRECATED!
* Marked specific specs for Audit Trail Consumption as deprecated because it must be reworked completely. Specs and changes on IHE ATNA Audit Messages are valid. [EPD-65]

1_12_EPR_PatientDeleteDocument !DEPRECATED!
* (ITI-62 Delete Document Set) not required anymore by TOZ (EPDV-EDI Anhang 2_Rev 1.1_DE.pdf) [EPD-121] 

1_14_EPR_PatientDeleteEPR
* References deprecated PatientDeleteDocument
* adjusted PPQ actors,transaction, tbd: can all policies for a paitent be deleted with Delete Policy Request?

2_01_EPR_CT
* change requirements to CT Profile for Swiss Time Service instead of ATNA (Requirements on CT Profile for Swiss Time Service)

2.2 EPR_HPGetDocuments
* XCPD needs not to be grouped with XUA [ITI-40] Provide X-User Assertion [EPR-SPID] (decision AG TSI meeting)

2.2 EPR_HPGetDocuments2of3
* XCPD needs not to be grouped with XUA [ITI-40] Provide X-User Assertion [EPR-SPID] (decision AG TSI meeting)

2_04_EPR_PatientAssignAccessRights
* adjusted PPQ actor/transaction

steps_pp_xds_reg2_of2
* XCPD needs not to be grouped with XUA [ITI-40] Provide X-User Assertion [EPR-SPID] (decision AG TSI meeting)

steps_ps_xds_reg2_of3
* XCPD needs not to be grouped with XUA [ITI-40] Provide X-User Assertion [EPR-SPID] (decision AG TSI meeting)

2_05_EPR_Patient_XDS-I_XCA-I_1of2
2_05_EPR_Patient_XDS-I_XCA-I_2of2
2_05_EPR_XDS-I_XCA-I_1of2
2_05_EPR_XDS-I_XCA-I_2of2
2_05_EPR_XDS-I_XCA-I
* added Note Maturity Level Specification/Revision started to each of the sequence diagrams

* added grouping actors (X-Service User, Provider) of [ITI-40] excplicit in all actors, affects all diagrams

# Changes after approval
11.7.2017 rename EPR-PID in EPR-SPID
11.7.2017 remove note in 1_02b
10.7.2017 EPR_CommunityInCircleOfTrust adjusted to CH:CPI, actor CPI_Client
10.7.2017 1_16 should not be a delete, to be clarified
10.7.2017 asynchronus nature of UPI communication corrected in 1_14, 1_16
8.6.2017  two new sequence diagrams EPD 2_02 PatientGetDocuments *** To be approved
7.6.2017: splitted sequence diagrams EPR 2_02 HP GetDocuments in three sequence diagram, in step 3 one arrow was missing for ITI-41
6.6.2017: new sequence diagram EPR 2.3b EPR_PatientStoreDocuments *** To be approved
3.6.2017: added CH:XUA to to the Authenticate User, Get X-User Assertion  Transaction
3.6.2017: added MPI_A-ID to ITI-41 EPR_HPStoreDocuments
3.6.2017: typo in 1_07_EPR-PatientCreateEPR

# Changes before publication 24.5.2017 after approval
removing notes and put the open notes in jira

# Changes for Sequence Diagrams after publication from 13.3.2017 including feedback from poll

Updated sequences diagrams will be made available before the next telco (24.4.2017)

## General changes

* wording: Changed "Cross Community" to "Other Communities" (18.3.2017, Request by JB)
* wording: Changed "EPD-PID" to "EPR-PID" (20.3.2017, Source: Nationale Integrationsprofile)
* wording: Changed "EPD" to "EPR" in all descriptions and files (22.3.2017, Source: Nationale Integrationsprofile)
* reviewed with ZAS and adjusted 1_07_CreateEPR, 1_14_DeleteEPR, new sequence diagrams 1_15_EPR_PatientEprQuery, 1_16_EPR_PatientEprInactivate (22.3.2017)

## Open Issues from David from 16.3
E-Mail from David from 16.3 about missing usescases.

1. 2.9.12, Register On-Demand Document Entry, ITI-61, Check with Tony Schaller first.
It is mentioned in 2_01_EPR_ATNA but after rereading it should be moved to 1_10_EPR_PatientVerifyAccessLog between step 16,17 and step 18,19 (the on-demand document gets generated according the query parameter the ITI-18 query).

2. 2.9.18, Querying ZAS with only demographic data, ITI-47, Use case missing
Querying ZAS with only demographic data (but not based on ITI-47) need to be clarified with a meeting with the people from ZAS. 

3. 2.9.19, PIX V3 Update Notification, ITI-46, Use case missing
David, Can you please provide an outline of a use case in what way ITI-46 Update Notification should be used? Then we can create accordingly a sequence diagram.

4. 2.9.29 Difference between synchromic and asynchromic communication with ZAS. When is SEDEX really needed? Are certificates (without SEDEX) sufficient to query the web services of ZAS? 
Need to be clarified with a meeting with the people from ZAS. 

1 done

2 done added new sequence diagram 

4 done ecH-0213, 0214 sedex certificate, CH-0215 needs sedex client, added as note to 1_14_EPR_PatientDeleteEPR 

3 done awaiting input

## 1_02_EPR_QueryingGovernmentServices

Walid [NO]: Usage of SVS (for CPI) is currently in question. Reinhold got the status quo. Maybe put on hold until final decision.

oe: Note that SVS is not yet confirmed for CPI

Monika [NO]:
> 1. Portals do not interact with CPI (remove 1-4, 9-12)

oe: Done
> 2. Secure Node (Community Components) needs to query CPI in order to find out if the other community is still part of the trusted communities.  (add new transaction)

oe: Discussion with Reinhold 11.4.2017: Secure Node is an IHE Actor an cannot query other community. What kind of and actor transaction should be added? TODO: Testcase missing,remove Community Portal and make own usecase with reinhold

> 3. Provider Information Directory (Community Components) needs to query CPI in order to retrieve the community prefix for LDAP (add new transaction)

oe: discussion with reinhold 11.4.2017, needs not to be that finegrained
> 4. New CH transactions PIDD will not be used on the portal (25,27). 

oe: DONE remove CH:PIDD from 25,27 
>The portal will query the HPD from the community first . 

> Comment: SV.S/CPI: 17 - 20: We've got feedback from stakeholders not to implement SVS for CPI. We're currently proving the proposal from Post/Swisscom/BINT
oe: see note above (comment to SVS). eHealth Suisse will propose an alternative solution and if that will be accepted, the sequence diagram will be adjusted

Reinhold [NO]: 
>See feedback from Monika; additional feedback: Testing certificates could be useful. Web service gateway expects certificates from Swiss Governement PKI with specific common name. Therefore I propose to include the authentication test case.

oe: discussion with reinhold 11.4.2017: no influence on testcase, should be tested at epd projectathon

DECISION: To be revised Sequence Diagram with comments above, otherwise approved 12.4.2017

## 1_02b_EPR_CommunityInCircleOfTrust

DECISION: Sequence Diagram Needs revision to be approved at 26.4.2017

## 1_03-1_6_EPR_Usecases

Walid [MAYBE]:
>Better title: HPD_Usecases. What about Provider Information Delta Download [CH:PIDD]? What about Provider Information Query [ITI-58] by Provider Information Consumer actor?

oe Done: title change. [CH:PIDD] is descriped in 1_02, ITI-58 are described in 1_02

Monika [NO]:
>1.5: Each community maintains their own HP/HO even if their are registered in other communites. The relation (cross-community) from one HP/HO to more than one community is not allowed anymore. If one HP/HO is registered in more than one community, each community maintains their own HPD entry for that HP/HO. The use case does not make sense because we do not have to demonstrate the relation of a HP to several communites. 

oe Done: Delete Usecase 1.5, clarified with reinhold 11.4.2017

Reinhold [NO]:
>See feedback from Monika

DECISION: To be revised Sequence Diagram with comments above, otherwise approved 12.4.2017

## 1_07_EPR_PatientCreateEPR
adjusted with feedback from ZAS (deleted first for transactions, clarified wording, deleted note)

Walid [NO]: 
>If [03] delivers back: "EPR-PID already present" Process needs to stop or fork because P. already has an EPR.
oe: add Fork if EPR-PID is already existing

Reinhold: add a new step eCH-0214 (Search person request) before eCH-0213 (talk with Hanspeter)?

>[07] also needs to feed the local-ID of the patient in the primary system
oe: local-ID is here not available at this step, resolved

Reinhold:
>01: Wording; "using" instead of "based on"; "ahvn13" instead of "avn13".

DECISION: Sequence Diagram Needs revision to be approved at 26.4.2017
Reinhold: add a new step eCH-0214 (Search person request) before eCH-0213 (talk with Hanspeter), NOT necessary (21.4.2017)
ACTION: DONE


## 1_08_EPR_PatientModifyAccessRights

Walid [NO]: 
>[14] seems to come too early. First the Policy needs to be fetched to the Policy Manager, then displayed on the portal, then modified [14], and then updated by Policy Manager 

oe: DONE, usecase was implied that they are displayed already, will be added for clarity

Reinhold:
>02-05: Only the CH:XUA Get X-User Assertion requires the SAML request/response according CH National Extension (ErgÃ¤nzung 1 zu Anhang 5 der EPDV-EDI) . For [02] we're requiring another specific SAML reqeust/response (SAML Artifact Binding) beween the IdP and the Portal (=Relying Party).

>03, 04, 11: according CH:XUA

oe: Discussion with Reinhold 11.4.2017, current sequence diagram has right text.

DECISION: To be revised Sequence Diagram with comments above, otherwise approved 12.4.2017


## 1_09_EPR_PatientModifyConfLevelDoc

Walid: 
>Just to keep in mind: X-Community Metadata Update is missing in nat. ext. but needs to come in next revision. 

DECISION: Sequence Diagram Approved 12.4.2017


## 1_10_EPR_PatientVerifiesAccessLog

### added [ITI-61] Register On-Demand Document Entry

Grouped Audit Record Repository with On-Demand Document Source
Added [ITI-61] Register On-Demand Document Entry within the both [ITI-18] queries

Walid:
>Seems correct to me. Validation by Tony needed.

Reinhold [NO]:
>According feedback from Tony, ITI-61 cannot be used here. The access log will not be registered in the EPD. 

OE: Access log is not registered within EPD. Remove ITI-61? ITI-61 Not necessary for an Registry with an On Demand Option, that means no On Demand Documen Source is necessary for Audit Record Repsoitory. (to be verfied by Eric)? 

>Both Document Registry and Document Consumer have to implement the On-Demand Option.

OE: Consumer On Demand Option has to be added to the actor, Document Registry only in the Document Audit Record Repository?

OE: Sequence Diagram Needs revision to be approved at 26.4.2017
ACTION: Eric review if ITI-61 / On Demand Document Source actor is not necessary for functionality of ATNA Audit Record Repository, OE Update Diagram


## 1_12_EPR_PatientDeleteDocument.txt

Walid: 
>Just to keep in mind: X-Community Delete Document Set is missing in nat. ext. but needs to come in next revision. 

Reinhold [NO]:
>19: Why not using ITI-62? 

OE: Clarify with Reinhold 11.4.2017, ITI-62 is in.
OE: Link to HP GetDoucments at the end of the transactions Done

DECISION: To be revised Sequence Diagram with comments above, otherwise approved 12.4.2017

## 1_14_EPR_PatientDeleteEPR
adjusted sequence diagram with feedback from ZAS 

Walid:
>Loop to delete documents might as well be done by proprietary transactions. We did not specify the usage of Delete Document Set. Also UPI will use an eCH-Standard-Message for broadcast (ask Reinhold for the number).

OE: Comment is resolved
OE: add "annulation message" in step03, done
OE: Sequence needs to be added to make an update on the MPI to delete the EPR-ID
OE: Delete the Policies from the Policy Repository

Reinhold:
>UPI informs other communities via broadcast, not depicted in this diagram

OE: Add a another communtiy where the broadcast message is received
OE: remove point 06, done
OE: note: optional transactions, done
OE: additional note, that tests for deletion of all data

DECISION: Sequence Diagram Needs revision to be approved at 26.4.2017


## 1_15_EPR_PatientEprQuery
new sequence diagram with feedback from ZAS 
OE/Reinhold/ZAS: clarify if transaction 3 includes also demographic data with ZAS or Resonse: DONE
OE: Walid will provide a footnote to the paragraph to the ordonance number about usage of SSN / EPR_PID
OE: transaction 1-4 should be closed (grahical issue box is prolonged), DONE

DECISION: Sequence Diagram Needs revision to be approved at 26.4.2017
ACTION: OE Update Diagram, Walid provide footnote


## 1_16_EPR_PateintEprInactivate
new sequence diagram with feedback from ZAS 
OE: second community as well
OE: replace actorn name UPI Client with UPI Clien: DONE
OE: same pattern as before, add MPI transaction (note:with other data has also be dealt with, should be consolidated) -> reference to PR_PatientDeleteEPR

DECISION: Sequence Diagram Needs revision to be approved at 26.4.2017
ACTION: OE Update Diagram 

## 2_01_EPR_ATNA 

### transactions [ITI-61] Register On-Demand Document Entry removed
[ITI-61] Register On-Demand Document Entry removed, because on On-Demand Document will be registered after a query ,see 1_10_EPR-PatientVerifiesAccessLog

DECISION: Sequence Diagram Approved 12.4.2017


## 2_01_EPR_CT

DECISION: Sequence Diagram Approved 12.4.2017


## 2_02_EPR_HPGetDocuments

### Transaction 36 
clarified note looping of initating gateway over responing gateways
>IHE TF1, Page 195,  Figure 18.3.3-1: XCA Detailed Interactions
>Here its clear that the ITI-18 looping is done with an initiating gateway and also described 

>IHE TF4 18.2.1 XDS Affinity Domain Option, 4795
>When receiving a Registry Stored Query from a local Document Consumer, shall require the homeCommunityId as an input parameter on relevant queries, and shall specify the homeCommunityId attribute within its Registry Stored Query responses. 

The point ist the relevant queries. For a few queries the patientid is not necessary in a xca context,and then the homeCommunityId is needed, but if the query is on a patient id, a homeCommunityId is not relevant for the looping. 

Walid:
>"Approved, but only roughly checked. Note between [19] and [20]: correct (btw: Until now I was not aware, that in the request from ext. community there will be a Document Consumer actor doing all the query and request work and collecting documents before handing them over to the responding gatway)"

DECISION: Sequence Diagram Approved 12.4.2017

## 2_03_EPR_HPStoreDocuments

DECISION: Sequence Diagram Approved 12.4.2017

## 2_04_EPR_PatientAssignAccessRights

Walid [NO]:
>I think [6] to [11] should be after [19] because Patient's MPI-Identity should be determined as early as possible (for logging purposes).
OE: Will stay in place, logging of portal ist done, not by patient

DECISION: Sequence Diagram Approved 12.4.2017

## 2_05_EPR_XDS-I_XCA-I

Walid [Not checked]:
>Juerg is the expert and it should resemble XDS/XCA (without "i")
Eric: Information that WADO will be deprecated, Eric will send information

DECISION: Sequence Diagram Approved 12.4.2017

