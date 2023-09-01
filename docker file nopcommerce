FROM mcr.microsoft.com/dotnet/sdk:7.0
LABEL author=khaja
RUN useradd -d /pavan --shell /bin/bash pavan
USER pavan
WORKDIR /pavan
COPY --chown=pavan:pavan nopCommerce /nopCommerce
ENV ASPNETCORE_URLS="http://0.0.0.0:5000"
EXPOSE 5000
WORKDIR /nopCommerce
CMD ["dotnet", "Nop.Web.dll"]