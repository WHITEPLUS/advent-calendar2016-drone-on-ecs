Drone on ECS
============

WHITEPLUS AdventCalendar2016のデモです。
[drone.io公式デモ](https://github.com/drone-demos/drone-on-ecs)の改造版。

Usage
-----
CertificateManagerのARN指定を行うパラメーターを追加しています。


    # params.json
    [
        {
            "ParameterKey": "VPC",
            "ParameterValue": "[VPC ID]"
        },
        {
            "ParameterKey": "Subnets",
            "ParameterValue": "[CSV LIST OF SUBNET IDS]"
        },
        {
            "ParameterKey": "CertificateArn",
            "ParameterValue": "[CertificateManager ARN]"
        },
        {
            "ParameterKey": "KeyName",
            "ParameterValue": "[KEYPAIR NAME]"
        },
        {
            "ParameterKey": "DroneRemoteDriver",
            "ParameterValue": "[DRONE REMOTE_DRIVER VALUE]"
        },
        {
            "ParameterKey": "DroneRemoteConfig",
            "ParameterValue": "[DRONE REMOTE_CONFIG VALUE]"
        }
    ]
    
    
