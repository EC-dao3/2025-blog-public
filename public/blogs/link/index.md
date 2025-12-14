代码示例：
const door = world.querySelector('#模型名字');
door.enableInteract = true;//允许交互/互动
door.interactHint = `靠近该模型显示的名字`;
door.interactRadius = 互动范围;
door.onInteract(async ({entity}) => {
  entity.player.link(
    '这里是你的链接', { isConfirm: false }
  );
});
ps：本代码仅适用于神岛，对了，不要填入危险链接哦~不然会被封号的~