# 300 - Package Layout

Ballerina encourages to have one microservice per package. In order to adhere to that rule, code to cloud generates only one container per package. These artifacts can be found in the ```target``` directory of the package. A complete representation of the package layout is as follows.

```
├── Cloud.toml                               
├── Ballerina.lock
├── Ballerina.toml
├── entry.bal 
├── modules (optional)
│   ├── foo
│   │   └── foo-0.0.1.bal
│   └── bar
│       └── bar-0.0.1.bal
└── target (auto-generated)
    ├── bala
    │   └── module-0.0.1.bala
    ├── bin
    │   └── <module>.jar
    ├── docker
    │       └── Dockerfile                        
    └── kubernetes
            └── <module>-0.0.1.yaml 
```

## 100 - Cloud.toml
See [README.md](./100/README.md)

## 200 - Ballerina.toml
See [README.md](./200/README.md)

## 300 - entry.bal
See [README.md](./300/README.md)

## 400 - modules (optional)
See [README.md](./400/README.md)

## 500 - target (auto-generated)
See [README.md](./500/README.md)
