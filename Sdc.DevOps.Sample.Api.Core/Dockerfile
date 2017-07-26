FROM microsoft/aspnetcore-build
WORKDIR /app

COPY *.csproj .
RUN dotnet restore

EXPOSE 50600
EXPOSE 50599

COPY . .
CMD dotnet publish --output /out/ --configuration Release
