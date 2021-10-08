(async () => {
  await ModMenu.init();
  const MenuTree = ModMenu.MenuTree;
  const MenuBool = ModMenu.MenuBool;
  const MenuButton = ModMenu.MenuButton;
  const coolInjMenu = new MenuTree('Cool Injectable Menu', [
    new MenuButton('Do Something Cool', () => alert('Something Cool!'));
    new MenuBool('Rocket Blasters Enabled', true);
    new MenuTree('Cool Settings', [
      new MenuButton('Launch Rocket!', () => {
        if(coolInjMenu[1].value){
          alert('Rocket launched!');
        } else {
          alert('Enable rocket blasters first!');
        }
      });
    ]);
  ])
  ModMenu.menu.arr.push(coolInjMenu);
})();
