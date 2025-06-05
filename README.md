# grpc-sso
1. cd .\proto\
2. go mod init proto

3. установка protoc для гошки:
https://grpc.io/docs/languages/go/quickstart/

Генерация прото файлов
                                                        сгенерированные файлы будут
                                                        иметь тот же пакет,            куда генерим
              путь до прото файла    куда генерим код   что и прото файлы              го grpc код                
protoc -I proto proto/sso/sso.proto --go_out=./gen/go --go_opt=paths=source_relative --go-grpc_out=./gen/go/ --go-grpc_opt=paths=source_relative