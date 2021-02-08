# SSLEngineSimpleDemo
:octocat: Amostra de código que ilustra o uso de um SSLEngine - O SSLEngine oferece flexibilidade aos desenvolvedores de aplicativos ao escolher estratégias de I/O e computação. Em vez de amarrar a implementação SSL/TLS a uma abstração de I/O específica (como SSLSockets de thread único), o SSLEngine remove as restrições de I/O e computação da implementação SSL/TLS.

O SSLEngineResult fornece uma grande quantidade de informações sobre o estado atual do SSLEngine. Este exemplo não examina todos os estados. Ele simplifica os problemas de I/O e threading a ponto de não ser um bom exemplo para um ambiente de produção; no entanto, é útil demonstrar a função geral do SSLEngine.

Um exemplo de uso do SSLEngine que simplifica a apresentação
removendo as questões de E / S e multithreading.

A demonstração cria dois SSLEngines, simulando um cliente e um servidor. A camada de "transporte" consiste em dois ByteBuffers: pense neles como tubos diretamente conectados.

Observe, este é um exemplo * muito * simples: o código real estará muito mais envolvido. Por exemplo, diferentes modelos de threading e I / O podem ser usados, os mecanismos de transporte podem fechar inesperadamente e assim por diante.

  * Quando este aplicativo é executado, observe que várias mensagens * (quebra / desempacotamento) passam antes que qualquer dado do aplicativo seja consumido ou * produzido. (Para obter mais informações, consulte as especificações SSL / TLS *.) Pode haver várias etapas para um handshake bem-sucedido *, portanto, é comum ver a seguinte série de operações:

### Uso

```
java SSLEngineSimpleDemo
```
