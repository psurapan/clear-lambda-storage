Clear Lambda code storage
===========================


Motivation
-----------
AWS limits the total code storage for Lambda functions to `75GB <https://docs.aws.amazon.com/lambda/latest/dg/limits.html#limits-list>`_.

The main reason of reaching such size is because for every deployment of existing function, AWS stores the previous version ("qualifier").

Usually, when you reach that point, you want to remove old version.
This tool will help you to!

1. Add the Lambda functions under qbi-mc-engine-code/functions/utils/handler.py
2. Use the serverless.yaml code to integrate with BRP serverelss infrastructure code (qbi-mc-engine-code/template.yaml)
