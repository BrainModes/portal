# Pilot Portal

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/agpl-3.0)

## Getting Started

### Frontend

This is the front end react application of Indoc Pilot project. The project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app). The back end is on `./server` folder.

#### Prerequisites

- nodejs: ^12.16.3
- npm: ^6.14.4

install both npm and nodejs on `https://nodejs.org/en/`

#### Install dependencies

run `npm i` on the `ROOT/` folder to install all the dependencies.

#### Config .env file

| Parameter                            | Description                                                                             | Default      |
| ------------------------------------ | --------------------------------------------------------------------------------------- | ------------ |
| REACT_APP_PORTAL_PATH                | root path for portal. you also need to update "homepage" in package.json to take effect | /pilot       |
| REACT_APP_BRANDING_PATH              | page path for your own branding page. logout/login/session expired                      | /pilot/login |
| REACT_APP_API_PATH                   | backend api endpoint for bff                                                            |
| REACT_APP_UPLOAD_URL                 | backend api endpoint for upload service                                                 |
| REACT_APP_DOWNLOAD_URL               | backend api endpoint for download service                                               |
| REACT_APP_DOWNLOAD_URL_V1            | backend api endpoint for download service v1                                            |
| REACT_APP_DEFAULT_AUTH_URL           | url for keycloak auth                                                                   |
| REACT_APP_KEYCLOAK_REALM             | keycloak realm                                                                          |
| REACT_APP_PLATFORM                   | Platform Name                                                                           | Pilot        |
| REACT_APP_DOMAIN_DEV                 | dev server domain                                                                       |
| REACT_APP_DOMAIN_STAGING             | staging server domain                                                                   |
| REACT_APP_DOMAIN_PROD                | prod server domain                                                                      |
| REACT_APP_SUPPORT_EMAIL              | user support email address                                                              |
| REACT_APP_PROXY_ROUTE                | proxy bff route when you are on local developing                                        |
| REACT_APP_XWIKI                      | xwiki path for all document                                                             |
| REACT_APP_ORGANIZATION_PORTAL_DOMAIN | your organization domain                                                                |
| REACT_APP_TEST_ENV                   | env for test cases, do not change this                                                  | dev          |
| REACT_APP_DcmSpaceID                 | DCM ID Title                                                                            | Dcm ID       |
| REACT_APP_dcmProjectCode             | Project used DCM ID                                                                     |

#### Run the Application

run `npm start` to start the React application. You can access the webpage on `localhost:3000` after it starts.

#### Build a Production Version

run `npm build`. After the compilation completed, the minimized static files are in `./build`. You can use any other backend to serve these files.

#### Terms of Use

The terms of use is in `public/files/terms-of-use.html`
