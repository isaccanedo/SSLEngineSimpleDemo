# SSLEngineSimpleDemo
:octocat: Amostra de código que ilustra o uso de um SSLEngine - O SSLEngine oferece flexibilidade aos desenvolvedores de aplicativos ao escolher estratégias de I/O e computação. Em vez de amarrar a implementação SSL/TLS a uma abstração de I/O específica (como SSLSockets de thread único), o SSLEngine remove as restrições de I/O e computação da implementação SSL/TLS.

O SSLEngineResult fornece uma grande quantidade de informações sobre o estado atual do SSLEngine. Este exemplo não examina todos os estados. Ele simplifica os problemas de I/O e threading a ponto de não ser um bom exemplo para um ambiente de produção; no entanto, é útil demonstrar a função geral do SSLEngine.

### Uso

```
java SSLEngineSimpleDemo
```
