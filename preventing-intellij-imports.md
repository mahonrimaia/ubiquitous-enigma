# Impedindo o IntelliJ de usar o * nos imports

Para impedir o IntelliJ IDEA de substituir seus imports com \*, você precisa configurar as preferências de **Class count to use import with ‘\*’** e **Names count to use static import with ‘\*’**:

Vá em **Settings** > **Editor** > **Code Style** > **Java**.  
Coloque um valor bem grande para ambas preferências, 500 por exemplo.  
E clique em **Apply** e **OK**.

![Printscreen showing those options in IntelliJ.](/assets/img001.png "Vá em Settings > Editor > Code Style > Java")