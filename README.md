### Participant

- auth
	- login w google
	- join link
	- run experiment

### ADMIN 

Minimal features

- auth
	- login
	- sign up
	- reset password
- admin user
	- username
	- password
	- name
	- alias
	- institution
	- phone or mail
	- description
	- etc
- projects
	- CRUD
	- join participant
		- link w hash
	- DTO
		- participants
		- description
		- alias
		- createdAt
		- updateAt
		- experiments
- Expirements
	- CRUD
	- DTO
		- uuid
		- enabled
		- tour
		- steps
		- alias
		- description
		- created_at
		- updated_at
	- tour - step by step
		- steps
			- step DTO
				- uuid
				- alias
				- type (screen, simple form, demo, task)
				- data
					- screen_uuid
					- js - webgazer - experiment feature
					- artefact_uuid (form)
	- artefacts
		- uuid
		- type (audio, picture, form)
		- created_at
		- updated_at
		- alias
		- used_by
			- screen__uuid
		- pictureData
			- url
		- audioData
			- src
		- formData
			- inputs
				- type (checkbox, text, textarea, radio group, select)
				- label
				- options
					- arr [ ]
						- label
						- value
	- screens
		- CRUD
		- screen DTO
			- uuid
			- alias
			- used_by
				- step__uuid
			- items
				- type (artefact, form )
				- position
				- area (heading, content, footer)
				- v_align
				- h_align 




### React Project minimal

- i18n (internationalization)
	- ptBr
	- enUs
- context api
	- auth / role
- react router dom
- ui lib
- axios
