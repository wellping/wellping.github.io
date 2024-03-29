# Study

A **study** is what the [participants](#participant--user) log in to and participate in.

It has a start date and an end date. [Pings](#ping) are sent regularly to the participant between the study's start date and end date.

It is uniquely identified by a study ID. You are encouraged to use a unique study ID for your study (e.g., use `collect_university_lab_study_fall_2020` instead of `my_study`).

A study file contains all information related to a study.

# Study File

A study file contains the following information.

## Study Info

The study info is the general info related to the study. For the definitions of the fields, see `_StudyInfoSchema` in [`StudyFile.ts`](https://github.com/wellping/study-schemas/blob/main/src/schemas/StudyFile.ts) or the available fields in the relavent fields in the [Well Ping Study File Editor](https://wellping.github.io/study-file-editor/).

## Streams (Question Streams)

A study can include multiple streams. Each stream is uniquely identified by an ID.

### Stream (Question Stream)

A stream contains a list of questions that will be presented to the user.

#### Question

A question is a single-screen question that the user will see.

# Ping

A ping refers to the a specific window of time where the participant will be able to complete a specific [stream](#stream-question-stream). The participant will receive a notification when a ping is active.

# Response / Answer

# Participant / User
