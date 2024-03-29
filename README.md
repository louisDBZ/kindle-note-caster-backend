# What is the purpose of this project?

Visit the complete documentation in `documentation-resources`>`Presentation` or click on this [link](documentation-resources/Presentation.md)

# How to run this project?

**Notebook prototype accessible in the folder kindle-note-caster-notebook**

# create an environment 

`py -3 -m venv venv`  ( note that the second `venv` is the name we gave to this environment)

For intelliji: edit configurations> Use specified interpreter

`venv\Scripts\activate` command to activate the environment. Then,` (venv) `  will be added in your terminal 

Then , create the file managing the environment variables:

```
DATABASE_HOSTNAME=
DATABASE_PORT=
DATABASE_PASSWORD=
DATABASE_NAME=
DATABASE_USERNAME=
SECRET_KEY=
ALGORITHM=
ACCESS_TOKEN_EXPIRE_MINUTES=
```

# RUN 

from the folder, `\kindle-note-caster\kindle-note-caster-api\app`, launch: `uvicorn main:app --reload`

# AuthN management

### AuthN management avec jwt/ Oauth2

to generate the key fot the security algorithm, to put in the .env: `openssl rand -hex 32`

# example for the config of the file_mapper.json file:

```json
{
"marketing": "Lecture/Marketing.docx",
"sales": "Lecture/Sales.docx"
}
```
# credits to this project

**No commercial use intended , check https://github.com/Sanjeev-Thiyagarajan/fastapi-course**


# RUN test

from the root of this project, launch `pytest`