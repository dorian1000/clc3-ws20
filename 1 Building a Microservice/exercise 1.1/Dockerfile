# Pull in the layer of the base image: golang:1.11-alpine 
FROM golang:1.11-alpine

# Set author label: LABEL author=[YOUR-EMAIL]
LABEL author='s1910595013@students.fh-hagenberg.at'

# Set working directory: `/opt`
WORKDIR ./

# Copy local file `main.go` to the working directory
COPY main.go ./

# List items in the working directory (ls -lsa) and show content of the `main.go`file (cat)
RUN ls -lsa && cat main.go

# Build the app (CGO_ENABLED=0 go build -o /usr/myapp) and show the /usr directory  (ls -lsa)
RUN CGO_ENABLED=0 go build -o /usr/myapp
RUN ls -lsa

