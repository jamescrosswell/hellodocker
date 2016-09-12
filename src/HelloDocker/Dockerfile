FROM microsoft/dotnet

MAINTAINER James Crosswell

# copies the output of our publish operation into the container
COPY	/bin/Release/PublishOutput /app
WORKDIR	/app

# make sure that port 500 is exposed
EXPOSE 5000

# now run the web application (self hosted with kestrel)
ENTRYPOINT ["dotnet", "HelloDocker.dll"]


