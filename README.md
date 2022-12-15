# FLEXBOX CSS
Estudando e conhecendo alguns elementos do flexbox no CSS.

## Antes de adicionar o flexbox

Originalmente antes de adicionar qualquer elemento no  nosso texto ele por padrão vem nesse formato.

![padrão](https://user-images.githubusercontent.com/101072311/207490525-79c0ec79-efb4-4c87-a18d-d626e91bb12d.png)

(Obs: Só foram adicionados cores no fundo e no container padding e boder-radius para melhor visualização.)

~~~CSS
body{
	background: linear-gradient(
    90deg,
    rgb(38, 37, 58) 0%,
    rgb(39, 39, 160) 35%,
    rgb(8, 149, 177) 100%
  );
}
~~~

~~~CSS
.container-1{ /*mesma config para os catainer-2 e container-3*/
	width: 15px;
 	height: 15px;
  background-color: rgb(90, 85, 134);
  border: 1px solid #fff;
  border-radius: 2px;
  padding: 2px;
}
~~~

#### Display: flex;

Assim que adiciona o display: flex; ela consegue identificar que a teg container vai ser o elemento do flexbox e assim eles já se organizam.

~~~CSS
.container{
	display: flex;
}
~~~

![displayFlex](https://user-images.githubusercontent.com/101072311/207490514-4f9f75ff-9d25-4ba1-88fe-c06596360714.png)

#### Flex-direction

Flex-direction ele serve para dizer qual vai ser o eixo principal, por padão ele vem flex-direction: row;

~~~CSS
.container{
	display: flex;
	flex-direction: row;
}
~~~

![displayFlex](https://user-images.githubusercontent.com/101072311/207490514-4f9f75ff-9d25-4ba1-88fe-c06596360714.png)

(flex-direction: row-reverse;)

![rowreverse](https://user-images.githubusercontent.com/101072311/207596142-bf57cad0-6739-4542-8149-3071409c9f34.png)

(flex-direction: column;)

![column](https://user-images.githubusercontent.com/101072311/207596152-5424d743-b9b3-4499-b0a7-f491cb91f169.png)

(flex-direction: column-reverse;)

![columnreverse](https://user-images.githubusercontent.com/101072311/207596158-d1874a21-187d-4f6a-9e1c-c6573a8b3725.png)

#### Justify-content

Justify-content ele ajuda a alinhar os elementos no eixo principal.

(justify-content: flex-start;)

![displayFlex](https://user-images.githubusercontent.com/101072311/207490514-4f9f75ff-9d25-4ba1-88fe-c06596360714.png)

(justify-content: flex-end;)

![flexend](https://user-images.githubusercontent.com/101072311/207600111-51ac6b9e-ffc4-472f-9986-d353dc97d164.png)

(justify-content: center;)

![center](https://user-images.githubusercontent.com/101072311/207601380-6dcb4859-5d90-4652-bf13-2e2677b8136c.png)

(justify-content: space-around;)

![spacearound](https://user-images.githubusercontent.com/101072311/207601415-cb153401-22ff-442c-a21b-5cb23d570cd2.png)

(justify-content: flex-start;)

![spacebetween](https://user-images.githubusercontent.com/101072311/207601404-151ed371-27be-472c-86de-7dca2fcadc25.png)

#### Align-items

Align-items ele vai servir para alinhar os elementos no eixo perpendicular.

(aling-items: flex-start;)

![center](https://user-images.githubusercontent.com/101072311/207601380-6dcb4859-5d90-4652-bf13-2e2677b8136c.png)

(aling-items: flex-end;)

![flexendaling](https://user-images.githubusercontent.com/101072311/207605535-4102319c-6493-4d44-bb24-ba3a44fa2201.png)

(aling-items: center;)

![centeraling](https://user-images.githubusercontent.com/101072311/207605503-650d6e7c-f7f8-4c02-9385-2e3be750df0d.png)

(align-items: stretch;)

![streach](https://user-images.githubusercontent.com/101072311/207605554-5101f4bc-5402-42a3-9313-dee5816ddc21.png)

(aling-items: baseline;)

![basealing](https://user-images.githubusercontent.com/101072311/207605568-a8e5b280-bbea-4f2a-9097-9e01ed4a5ee2.png)

#### Flex-wrap

você utiliza o flex-wrap para se decidir se os elementos irão para a linha de baixo quando chegarem no final ou se ficarão apertados.

Por padrão ele já vem no formato nowrap
(flex-wrap: nowrap;)

![rowwrep](https://user-images.githubusercontent.com/101072311/207609220-db0aa73e-346b-4fb1-91fc-03bcef7be082.png)

(flex-wrap: rep;)

![wrap](https://user-images.githubusercontent.com/101072311/207609226-013f7dac-d828-452c-a26f-5e2d5c3532ba.png)

##### Flex-flow

você pode fazer a junção do flex-direction e flex-wrap.

(flex-flow: row wrap;)

![wrap](https://user-images.githubusercontent.com/101072311/207609226-013f7dac-d828-452c-a26f-5e2d5c3532ba.png)

#### Align-content

Usamos quando existe o flex-wrap e queremos alinhar com o nosso eixo perpendicular.

(aling-content: flex-start;)

![contentflexstart](https://user-images.githubusercontent.com/101072311/207612608-19ba5fdc-de69-41d7-9c30-0b7419a08b6a.png)

(aling-content: flex-end;)

![contentflexend](https://user-images.githubusercontent.com/101072311/207612618-0dbbee49-1d6c-4155-8bdb-2574cdaf4588.png)

(aling-content: center;)

![contentcenter](https://user-images.githubusercontent.com/101072311/207612632-d1a7bba7-46c3-4c5e-bb6c-be5266bf19d1.png)

(aling-content: space-between;)

![spacebetcontent](https://user-images.githubusercontent.com/101072311/207612643-b348cddf-e4ea-47da-933b-69de8a06536e.png)

(aling-content: space-around;)

![around](https://user-images.githubusercontent.com/101072311/207612654-fa7fdaaf-0c30-48d6-89ab-cd569fdfb8d7.png)

#### gap, row-gap e column-gap
Utilizando essas propriedades você consegue fixar algum tamanho entre os elementos, sejam eles lado a lado ou entre eles em cada linha.


(row-gap: 10px;)

![rowgap](https://user-images.githubusercontent.com/101072311/207615029-ef52bfe8-1feb-4d9c-b33a-d6daae2b742b.png)

(column-gap: 30px;)

![columngap](https://user-images.githubusercontent.com/101072311/207615283-a4de1060-e24e-4f76-9517-cc5b17680914.png)

(gap: 10px 30px;)

![gap](https://user-images.githubusercontent.com/101072311/207614990-90cb78e8-0910-4f76-aff7-eaf4c1f68ee0.png)

~~~CSS
.container {
  color: #fff;
  display: flex;/*Para identificar que a teg container vai ser o elemento do flexbox*/
  flex-direction: row;
  justify-content: center;
 
  align-items: center;
  flex-wrap: wrap;
  align-content: center;
  row-gap: 10px;
  column-gap: 30px;

}
~~~


## Ferramentas e Tecnologias usadas nesse repositório 🧱
<div style="display: inline_block"><br>

<img align="center" alt="Augusto-HTML" height="50" width="50" src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/html5/html5-plain.svg">
<img align="center" alt="Augusto-CSS" height="50" width="50" src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/css3/css3-original.svg">

</div>    

## Teste o projeto 👁‍🗨

Download do projeto para testar em sua máquina: https://github.com/AugustoMello09/FLEXBOX-CSS/archive/refs/heads/main.zip

## Entre em contato comigo através dos canais abaixo e desde já, agradeço a atenção. 🤝 

<div>

  <a href="https://www.linkedin.com/in/jos%C3%A9-augusto-794a94234/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
 <a href="mailto:joseaugusto.Mello01@gmail.com" target="_blank"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>   

  </div>
