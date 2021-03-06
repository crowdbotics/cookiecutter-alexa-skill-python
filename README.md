# Cookiecutter Alexa-skill Python

**Cookiecutter** template for an Alexa skill in Python.

## Requirements

- Cookiecutter : `pip install -U cookiecutter`

## Steps

- Create a repo on [Github](https://github.com/new) with a desired [REPOSITORY] name (for example : alexa-skill-my-new-skill)
- Fill the short description on Github and copy it for the following steps
- Execute in the terminal `git clone https://github.com/tducret/[REPOSITORY].git`
- Execute the cookiecutter with `cookiecutter -f https://github.com/tducret/cookiecutter-alexa-skill-python.git` (`-f` is to overwrite the contents of the output directory if it already exists)
- `cd [REPOSITORY]`
- Update README.md
- Create an [icon](https://developer.amazon.com/fr/docs/tools/icon-builder.html) for your skill and save it to `icons` folder
- Create a virtual environment to get the needed packages : `virtualenv venv; source venv/bin/activate; pip install ask-sdk`
- When everything is in place, add the files to git, commit it and push it : `git add .; git commit -am "First commit"; git push`
- Add topics (keywords) related to the project on Github (finding your project will be easier)
- Go to [Alexa development console](https://developer.amazon.com/alexa/console/ask) to create the new skill
- You may extract the content of the interaction schema with the `JSON Editor` button, and save it to `speech_assets/interactionSchema.json` 
- Go to [AWS Lambda console](https://eu-west-1.console.aws.amazon.com/lambda/home?region=eu-west-1) to create the new function, and upload the zip produced with `package.sh`
