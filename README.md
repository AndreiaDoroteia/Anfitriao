# Anfitrião

Queremos apresentar a solução ideal para os seus problemas.
Com esta plataforma queremos inovar o sistema de reservas rústico atualmente presente
em muitas das empresas relacionadas com o Turismo e Hotelaria em Portugal. As nossas soluções foram investigadas e debatidas de forma a proporcionar uma eficácia e eficiência à tanto tempo desejadas.
Vamos recrear um sistema que permita fazer a gestão de uma forma mais dinâmica e apelativa não só aos funcionarios como também aos utilizadores menos familiarizados com a informática.

*O nosso sistema vai-se chamar Anfitrião*.

Segundo o dicionário:

*Pessoa que demonstra interesse em pagar ou paga os gastos de um jantar, banquete, festa etc.
Indivíduo que recebe pessoas ou as convida para vários eventos em sua própria casa.*

Nós identificamo-nos com esta definição e partilhamos desta visão por tanto, queremos que se sinta como em casa quando estiver a dispôr da nossa plataforma!

Para dar a entender melhor as funcionalidades do *Anfitrião* dividimos-as em duas categorias tendo em conta as funcionalidades de maior importância para as de menos relatividade:

#### Must Have
   1. Realizar  Reservas.
   2. Eliminar  Reservas.
   3. Modificar Reservas.
   4. Vizualização das Reservas.

#### Nice to Have
   1. Gerar PDF com informações referentes às reservas de um cliente específico se solicitado.
   2. Aplicação Mobile.

Com este documento pretendemos establecer os objetivos a alcançar durante
o projeto de aula para os módulos que seguem de java na Atec.
Para começar será criado um Diagrama de Classes chamado UML.

#### Classes:
 ``` Java
public class Pessoa{
    int id;
    String nome;
    String dataNascimento;
    String cartaoCidadao;
}
 ```
 ``` Java
public class Cliente extends Pessoa{
  ArrayList<Reserva> Reservas;
  String Observacoes;
}
 ```

 ``` Java
public class Funcionarios extends Pessoa{
  String funcao;
  int salario;
}
```

 ``` Java
public class Reserva{
  int id;
  Cliente x;
  Quarto y;
  Date inicio;
  Date final;
}
 ```

 ``` Java
public class Quarto{
    int id;
    boolean camaCasal;
    int camaSolteiro;
    int numMaxPessoas;
    boolean ocupado;
    boolean reservado;
  }
 ```
