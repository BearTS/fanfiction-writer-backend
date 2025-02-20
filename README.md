<p align="center">
<a href="https://dscvit.com">
	<img width="400" src="https://user-images.githubusercontent.com/56252312/159312411-58410727-3933-4224-b43e-4e9b627838a3.png#gh-light-mode-only" alt="GDSC VIT"/>
</a>
	<h2 align="center"> < Insert Project Title Here > </h2>
	<h4 align="center"> < Insert Project Description Here > <h4>
</p>

---
[![Join Us](https://img.shields.io/badge/Join%20Us-Developer%20Student%20Clubs-red)](https://dsc.community.dev/vellore-institute-of-technology/)
[![Discord Chat](https://img.shields.io/discord/760928671698649098.svg)](https://discord.gg/498KVdSKWR)

[![DOCS](https://img.shields.io/badge/Documentation-see%20docs-green?style=flat-square&logo=appveyor)](INSERT_LINK_FOR_DOCS_HERE) 
  [![UI ](https://img.shields.io/badge/User%20Interface-Link%20to%20UI-orange?style=flat-square&logo=appveyor)](INSERT_UI_LINK_HERE)

## Implemented Features(Remove once complete)
- [x] Healthcheck
- [x] Error Responses for status codes 500(server error), 404(notfound), 405(methodnot), 400(badrequest), 422(failvalidation)
- [x] Helper functions for read/write JSON
- [x] Validation package for email, struct fields, etc
- [ ] Email for activation token
- [ ] Middleware
  - [ ] Auth
  - [ ] Rate limiter
  - [ ] Panic Recovery
- [ ] Resend activation email 
- [x] Routes
  - http.MethodGet, "/v1/healthcheck", app.healthcheckHandler
  - http.MethodGet, "/v1/labels/:id", app.showLabelHandler
  - http.MethodPost, "/v1/labels", app.createLabelHandler
  - http.MethodDelete, "/v1/labels/:id", app.deleteLabelHandler
  - http.MethodPost, "/v1/users", app.registerUserHandler
  - http.MethodPut, "/v1/users/activated", app.activateUserHandler
- [x] Labels
  - [x] Create Label Handler + DB
      - [x] Sublabel and blacklist autocalled, as well as standalone funcs
      - [ ] Specific error message instead of generic for passing created label id as a sublabel/blacklist
      - [ ] \ Error message for passing labels that don't exist (quietly ignored)
      - [ ] \ Change sublabel/blacklist to take in names instead of IDs
      - [ ] Figure out how to handle cases where partial creation is done in DB
  - [x] Get Label Handler + DB
      - [x] Sublabel and blacklist autocalled, as well as standalone funcs
      - [x] Get list of all labels
  - [x] Update Label name (all references to other tables will be create/delete only)
  - [x] Delete Label Handler + DB
      - [x] On Delete Cascade auto deletes sublabels/blacklist
  - [x] Delete Sublabel/Blacklist DB func
      - If list of IDs passed, only those deleted, else all are deleted
- [x] Users 
  - [x] Create User Handler + DB
  - [ ] Email sending
  - [x] User activation
  - [ ] Session tokens
- [ ] Events
  - [x] DB
  - [ ] Handler
- [ ] Timelines
  - [x] DB
  - [ ] Handler
- [ ] Stories  
  - [x] DB
  - [ ] Handler

## Features
- [ ]  < feature >
- [ ]  < feature >
- [ ]  < feature >
- [ ]  < feature >

<br>

## Dependencies
 - < dependency >
 - < dependency >


## Running


< directions to install > 
```bash
< insert code >
```

< directions to execute >

```bash
< insert code >
```

## Contributors

<table>
	<tr align="center">
		<td>
		John Doe
		<p align="center">
			<img src = "https://dscvit.com/images/dsc-logo-square.svg" width="150" height="150" alt="Your Name Here (Insert Your Image Link In Src">
		</p>
			<p align="center">
				<a href = "https://github.com/person1">
					<img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36" alt="GitHub"/>
				</a>
				<a href = "https://www.linkedin.com/in/person1">
					<img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36" alt="LinkedIn"/>
				</a>
			</p>
		</td>
	</tr>
</table>

<p align="center">
	Made with ❤ by <a href="https://dscvit.com">GDSC-VIT</a>
</p>
