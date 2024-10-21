# Dockerfile for Rust API
FROM rust:1.82.0

WORKDIR /app

# Copy the application code
COPY . .

# Build dependencies
RUN cargo fetch

# Build the application
RUN cargo build --release

# Expose the port on which the API runs
EXPOSE 8000

# Start the application
CMD ["./target/release/sdv_api"]
