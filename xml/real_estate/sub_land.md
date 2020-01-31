### Subcategoria `Terrenos, sítios e fazendas`

Para esta subcategoria, é necessário preencher o parâmetro `<SubTipoImovel>` com os seguintes valores:

| `<SubTipoImovel>` | Título do anúncio |
|-------------------------|-----------------------|
| `Loteamento Condomínio` | Loteamento/condomínio |
| `Loteamento Padrão` | Loteamento/condomínio |
| `Sítio` | Sítio |
| `Sítio Chácara` | Sítio |
| `Sítio Rural` | Sítio |
| `Terreno` | Terreno |
| `Terreno Padrão` | Terreno |
| `Chácara` | Chácara |
| `Chácara Rural` | Chácara |
| `Fazenda` | Chácara |
| `Fazenda Rural` | Chácara |
| `Haras` | Chácara |
| `Haras Rural` | Chácara |

Caso não seja enviado nenhum valor para `<TituloAnuncio>`, será montado um título para o anúncio baseado no `<SubTipoImovel>` e outros atributos, como número de quartos, localização, etc. 

Aqui está um exemplo de XML para inserção ou edição de anúncios na subcategoria `Terrenos, sítios e fazendas`:

```xml
<?xml version="1.0" encoding="utf-8"?>
<Carga xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <Imoveis>
        <Imovel>
            <CodigoImovel>FAZENDA001</CodigoImovel>
            <TituloAnuncio>Fazenda do Petrus</TituloAnuncio>
            <SubTipoImovel>Fazenda Rural</SubTipoImovel>
            <Cidade>Promissão</Cidade>
            <Bairro>Capituva</Bairro>
            <CEP>16370000</CEP>
            <PrecoVenda>5000000</PrecoVenda>
            <ValorIPTU>5000</ValorIPTU>
            <AreaTotal>100000</AreaTotal>
            <Observacao>A melhor fazenda de Promissão, prontinha para você morar com suas ovelhas dorper!\nFica perto de um parque bem grande, cheio de árvore.\nMuito legal, você deveria visitar!</Observacao>
            <Fotos>
                <Foto>
                    <URLArquivo> http://www.site_da_imobiliaria.com/foto_legal.jpg</URLArquivo>
                </Foto>
                <Foto>
                    <Principal>1</Principal>
                    <URLArquivo> http://www.site_da_imobiliaria.com/foto_legal2.jpg</URLArquivo>
                </Foto>
            </Fotos>
        </Imovel>
    </Imoveis>
</Carga>
```