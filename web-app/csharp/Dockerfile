# Build stage using Bitnami's dotnet SDK image
FROM bitnami/dotnet-sdk:8.0.407 as build

WORKDIR /app

# Copy csproj and restore
COPY *.csproj .
RUN dotnet restore

# Copy rest of the code and publish
COPY . .
RUN dotnet publish -c Release -o out

# Runtime stage — use same image or aspnet-only image if needed
FROM bitnami/dotnet-sdk:8.0.407

WORKDIR /app
COPY --from=build /app/out .

EXPOSE 5052
ENTRYPOINT ["dotnet", "csharp.dll"]
