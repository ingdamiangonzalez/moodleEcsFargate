# Moodle con ECS (fargate) y RDS

## Qué resuelve este reopsitorio?

La idea de este proyecto es poder desplegar con un solo click la plataforma de educación "Moodle" en AWS utilizando para esto los dockers creados por Bitnami (https://github.com/bitnami/bitnami-docker-moodle), un cluster de ECS y una base de datos RDS.

### Arquitectura

[![Arquitectura](images/arquitectura.png)]

| Region    | Nombre                | Crear                                                                                                                                                                                                                                                 |
| --------- | --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| us-east-1 | US East (N. Virginia) | [![cloudformation-launch-stack](images/cloudformation-launch-stack.png)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=Moodle&templateURL=https://deploymoodleecs.s3.amazonaws.com/moodleEcsFargate.yaml) |
