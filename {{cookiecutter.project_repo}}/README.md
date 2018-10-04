# Skill Alexa {{cookiecutter.skill_name}}

## Description

![{{cookiecutter.skill_name}} Alexa skill icon](/icons/icon_108.png)

{{cookiecutter.project_short_description}}

# Release note

## v0.1.0 - XX/XX/XXXX

### Usage

You can ask 

> - Alexa, demande à {{cookiecutter.skill_name}}...
> - ...


-------------------------------

## Requirements

IF NEEDED

## Useful

- [Alexa developer console](https://developer.amazon.com/alexa/console/ask)
- [AWS Lambda console](https://eu-west-1.console.aws.amazon.com/lambda/home?region=eu-west-1)
- [Icon generation](https://developer.amazon.com/fr/docs/tools/icon-builder.html)

### Alexa developer console

- Add at least one intent
- If needed, go to `Interfaces` to enable `Audio Player` and `Display Interface`
- Don't forget to save and build the model

### Lambda 

- Alexa skill kit is not available in Paris AWS datacenter (available in Ireland)
- Load the zip file obtained in `build` (generated with `package.sh`)
- Make sure you put `{{cookiecutter.skill_slug}}_skill.handler` in Gestionnaire
- Select **Alexa Skills Kit** in `Designer`
- Put the skill id that you got from the `Alexa developer console` > Endpoint
- Copy the ARN of the function from the upper right corner
- Paste it in > Endpoint > Default Region in `Alexa developer console`

## TODO

- [ ] 