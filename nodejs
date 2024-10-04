const readline = require('readline');

let Herois = [
    { nome: "Messiah", xp: 700 },
    { nome: "Randvi", xp: 1200 },
    { nome: "Ragnar", xp: 3409 },
    { nome: "Thorfinn", xp: 5288 },
    { nome: "Bjorn", xp: 6158 },
    { nome: "Kaidan", xp: 7999 },
    { nome: "Shepherd", xp: 8522 },
    { nome: "Price", xp: 9198 },
    { nome: "Soap", xp: 10031 },
];

const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

// Pergunta ao usuário qual herói ele deseja escolher
rl.question('Por favor, escolha um herói (ex: Messiah, Randvi, Ragnar, Thorfinn, Bjorn, Kaidan, Shepherd, Price, Soap): ', (nomeHeroi) => {
    
    // Inicializa a variável para armazenar o herói escolhido
    let heroiEscolhido;

    // Loop para encontrar o herói
    for (let i = 0; i < Herois.length; i++) {
        if (Herois[i].nome.toLowerCase() === nomeHeroi.toLowerCase()) {
            heroiEscolhido = Herois[i];
            break; // Sai do loop se encontrar o herói
        }
    }

    // Verifica se o herói foi encontrado
    if (heroiEscolhido) {
        let nivel;

        // Estrutura switch case para determinar o nível
        switch (true) {
            case (heroiEscolhido.xp < 1000):
                nivel = 'Ferro';
                break;
            case (heroiEscolhido.xp >= 1001 && heroiEscolhido.xp <= 2000):
                nivel = 'Bronze';
                break;
            case (heroiEscolhido.xp >= 2001 && heroiEscolhido.xp <= 5000):
                nivel = 'Prata';
                break;
            case (heroiEscolhido.xp >= 5001 && heroiEscolhido.xp <= 7000):
                nivel = 'Ouro';
                break;
            case (heroiEscolhido.xp >= 7001 && heroiEscolhido.xp <= 8000):
                nivel = 'Platina';
                break;
            case (heroiEscolhido.xp >= 8001 && heroiEscolhido.xp <= 9000):
                nivel = 'Ascendente';
                break;
            case (heroiEscolhido.xp >= 9001 && heroiEscolhido.xp <= 10000):
                nivel = 'Imortal';
                break;
            default:
                nivel = 'Radiante';
                break;
        }

        // Exibe a mensagem final
        console.log(`O Herói de nome ${heroiEscolhido.nome} está no nível de ${nivel}`);
    } else {
        console.log('Herói não encontrado. Por favor, escolha um herói válido.');
    }

    rl.close();
});
