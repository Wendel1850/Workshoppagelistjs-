# Workshoppagelistjs-
// Função para exibir a lista de workshops
function exibirWorkshops() {
  const workshops = [
    {
      titulo: 'Workshop de JavaScript',
      descricao: 'Um workshop sobre JavaScript para iniciantes',
      data: '2023-03-15',
      hora: '14:00',
      local: 'Auditório da empresa'
    },
    {
      titulo: 'Workshop de HTML e CSS',
      descricao: 'Um workshop sobre HTML e CSS para iniciantes',
      data: '2023-03-22',
      hora: '10:00',
      local: 'Sala de treinamento'
    },
    {
      titulo: 'Workshop de React',
      descricao: 'Um workshop sobre React para desenvolvedores',
      data: '2023-03-29',
      hora: '14:00',
      local: 'Auditório da empresa'
    }
  ];

  const listaWorkshops = document.getElementById('lista-workshops');

  workshops.forEach((workshop) => {
    const item = document.createElement('div');
    item.innerHTML = `
      <h2>${workshop.titulo}</h2>
      <p>${workshop.descricao}</p>
      <p>Data: ${workshop.data}</p>
      <p>Hora: ${workshop.hora}</p>
      <p>Local: ${workshop.local}</p>
    `;
    listaWorkshops.appendChild(item);
  });
}

// Chama a função para exibir a lista de workshops
exibirWorkshops();
