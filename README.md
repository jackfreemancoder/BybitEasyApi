<?xml version="1.0" encoding="utf-8"?>
<package xmlns="http://schemas.microsoft.com/packaging/2013/05/nuspec.xsd">
  <metadata>
    <id>BybitApi.Net</id>
    <version>1.24.6</version>
    <authors>Jack Freeman</authors>
    <license type="expression">MIT</license>
    <licenseUrl>https://licenses.nuget.org/MIT</licenseUrl>
    <icon>icon.png</icon>
    <readme>README.md</readme>
    <projectUrl>https://github.com/jackfreemancoder/BybitEasyApi</projectUrl>
    <description>Bybit is a client library designed to interact with the Bybit REST and Websocket APIs. It translates all data into easy-to-understand models and enum values. Key features include automatic websocket connection and reconnection management, a client-side order book implementation, seamless integration with other exchange client libraries, and more.</description>
    <tags>Bybit Bybit.Net Bybit.com Bybit Client Bybit API CryptoCurrency CryptoCurrency Exchange</tags>
    <repository type="git" />
    <dependencies>
      <group targetFramework="net8.0">
        <dependency id="CryptoExchange.Net" version="9.1.0" exclude="Build,Analyzers" />
      </group>
      <group targetFramework=".NETStandard2.0">
        <dependency id="CryptoExchange.Net" version="9.1.0" exclude="Build,Analyzers" />
      </group>
      <group targetFramework=".NETStandard2.1">
        <dependency id="CryptoExchange.Net" version="9.1.0" exclude="Build,Analyzers" />
      </group>
    </dependencies>
  </metadata>
</package>
