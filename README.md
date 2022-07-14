# libapps
Custom styling and configuration documentation for Springshare apps.

Note: DLSS is not formally the "owner" of these applications, but we often get called to support various tasks or features related to them.

## [LibGuides](https://guides.library.stanford.edu/)

* Templates are in the `libguides` directory for header, footer, etc.
* Staff documentation exists in [Google Drive](https://drive.google.com/open?id=0APSFtg1s6VIjUk9PVA).
* Access team did some accessibility testing, but extent is not clear; perhaps look at the [CSS changelog](https://docs.google.com/document/d/1ZHIqeaIihgJsjPd3yhJ_sRlJz-0t3d2O0WdoVoYdFEQ/edit)

## [LibCal](https://appointments.library.stanford.edu/)

* Templates are in the `libcal` directory for header, footer, etc.
* Staff documentation in [Google Drive](https://drive.google.com/open?id=0ACfyS05ZK9O6Uk9PVA).
* Access Team undertook [accessibility testing](https://docs.google.com/document/d/1AC2c1PYu771NHGnp_8rFeBIarxO8ZTIuMDGDA-K3ml4/edit):
  * August 2021: Camille tested only the appointment scheduler-related features
* LibCal requires [integration with Azure's OAuth2 provider](https://ask.springshare.com/libcal/faq/2036) to enable calendar sync with Outlook. Ashley Jester set this up originally but left Stanford in May 2022.

## [LibApps](https://stanforduniversity.libapps.com/)

LibApps is the admin control panel for the Springshare suite.

* To create a new admin, first create the user an account in one of the related systems (e.g. LibGuides/LibCal).

### LibAuth

[LibAuth](https://ask.springshare.com/libapps/faq/609) is Springshare's integration with organizational SSO. We are currently using the SAML/Shibboleth integration.

Springshare is a member of the InCommon Federation, which makes set up of the Shibboleth service provider (SP) fairly easy in terms of Stanford. See more information at the [MaIS Confluence page on SSO/SAML login with vendor systems](https://asconfluence.stanford.edu/confluence/pages/viewpage.action?pageId=1156940377).

As a third party system we think that Springshare/LibAuth falls under the [UIT attribute release policy for InCommon Research and Scholarship](https://uit.stanford.edu/service/saml/arp/incommon), rather than the general [SAML ARP](https://uit.stanford.edu/service/saml/arp). What this means in practice is that we have access to [`eduPersonAffiliation`](https://uit.stanford.edu/service/saml/arp/edupa), and not [`suAffiliation`](https://uit.stanford.edu/service/registry/data-affiliation-types-qualifiers)'s list of privilege groups.

## [LibStaffer](https://stanford.libstaffer.com/)

LibStaffer is a staff-only tool used to schedule shifts.

## [LibWizard](https://termanengineering.libwizard.com/)

LibWizard is a survey/forms tool. It's only in use by Terman to our knowledge.

