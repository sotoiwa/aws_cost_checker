# aws_cost_checker

## Usage

Create `lambda.json`.

```json
{
  "name": "aws_cost_checker",
  "description": "My AWS cost checker.",
  "region": "ap-northeast-1",
  "runtime": "python3.7",
  "handler": "lambda_function.lambda_handler",
  "role": "arn:hogehoge",
  "timeout": 300,
  "memory": 128,
  "variables":
    {
      "SLACK_WEBHOOK_URL": "https://hogehoge",
      "SLACK_CHANNEL": "#hogehoge"
    }
}
```

Install lambda-uploader.

```shell
pip3 install lambda-uploader
```

Upload function.

```shell
cd aws_cost_checker
lambda-uploader
```
