# Start from the official Go image
FROM golang:1.22.1

# Set the working directory inside the container
WORKDIR /app

# Copy Go module files first
COPY go.mod .

# Then copy the source file
COPY main.go .

# Download dependencies (none in this case, but good practice)
RUN go mod download

# Build the Go app
RUN go build -o main .

# Run the binary
CMD ["./main"]