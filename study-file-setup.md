# Set Up Your Study File

Your study file is a [YAML](https://yaml.org/) file or a [JSON](https://www.w3schools.com/whatis/whatis_json.asp) file that contains all information (e.g. question streams, start and end dates, hour(s) to send pings each day) related to your study.

## Definitions

See [Glossary](./glossary.md).

## Create a Study File

### GUI Interface

If you want to easily create a study file, consider using the **[Well Ping Study File Editor](https://wellping.github.io/study-file-editor/)**. With this editor, you can create, save, and load an editor file, and eventually export the editor file as a JSON study file that could be used by Well Ping.

*Note: The editor is incomplete as of now and may not support all features in Well Ping.*

#### Example Editor Files

TODO

### Manual Creation

Alternatively, you may also create a study file manually in JSON or YAML. You need to understand JSON or YAML. To see the exact format the JSON or YAML file should be in, refer to the source code of [`StudyFile.ts`](https://github.com/wellping/study-schemas/blob/main/src/schemas/StudyFile.ts) and related files.

#### Example Study Files

See [Example Study Files](./example-study-files/).

## Can the study file be updated after some participants have already logged in?

When the participant logs in in Well Ping, they downloads your study file and stores it locally. At every subsequent launch of the app, Well Ping will fetch the study file again from your server in the background and use the newly downloaded study file at the next launch.

As such, it is possible to update the study file even when some participants have already logged in. They will be using the new study file at the second launch of Well Ping after the study file update. However, we only recommend updaing study files to fix smaller issues such as typos, and not to change larger components such as streams as larger changes might create unpredictable problems.
