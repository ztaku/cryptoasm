# CryptoAsm
CryptoAsm�͉��z�A�Z���u���ł��B  
���s�ł��閽�߂͂P�A�f�[�^�̈ړ������ł��B  
C����̃|�C���^�̗����ɖ𗧂��܂��B

## ���W�X�^
���W�X�^�ɂ�a��p������܂��Bp�̓������̃A�h���X���w�������܂��B

    mov p,a

p���W�X�^��a���W�X�^�̒l�����܂��B

## ���l
    mov a,1

a���W�X�^�ɐ��l�̂P�����܂��B

## ������
�������ɂ�0�Ԓn����6�Ԓn������܂��B�����Ƀf�[�^���i�[���܂��B
�Ԓn�̂��Ƃ��A�h���X�Ƃ������܂��B

## �ϐ�
�ϐ�i,j,k�Ɣz��l���g���܂��B
�ϐ�i�̓�������0�Ԓn�Aj��1�Ԓn�Ak��2�Ԓn�ɒl���i�[���܂��B

    mov j,a

a���W�X�^�̒l��ϐ�j�A�܂胁������1�Ԓn�Ɋi�[���܂��B

    mov a,k

�ϐ�k�A�܂胁������1�Ԓn�̒l��a���W�X�^�ɓ���܂��B

## �z��
�z��l��l[0],l[1],l[2]������A
���ꂼ��3�Ԓn�A4�Ԓn�A5�Ԓn�ł��B

    mov a,l[1]

�z��l[1]�܂胁����4�Ԓn�̃f�[�^��a���W�X�^�ɓ���܂��B

    mov l[0],a

a���W�X�^�̒l��z��l[0]�܂胁����3�Ԓn�Ɋi�[���܂��B

## �|�C���^
p���W�X�^�̓A�h���X��ێ����A���̃A�h���X�Ɋi�[���ꂽ�f�[�^��
�A�N�Z�X�ł��܂��B

    mov p,1
    mov a,*p

p���W�X�^��1�����܂��B
a���W�X�^��1�Ԓn�̓��e������܂��B

1�Ԓn�̓��e��10�̎���10���A
1�Ԓn�̓��e��20�̎���20���Aa���W�X�^�ɂ���܂��B

    mov p,2
    mov *p,a

p���W�X�^��2�����܂��B
2�Ԓn��a���W�X�^�ɂ̓��e������܂��B

## �|�C���^ 2

    mov p,2
    mov *p+1,a

p��2�����܂��B
�����1�𑫂����A�h���X�A�܂�3�Ԓn��a���W�X�^�̒l���i�[���܂��B

## �A�h���X
�ϐ��̃A�h���X�����o���܂��B

    mov p,&j

p���W�X�^�ɕϐ�j�̃A�h���X����܂��B
�ϐ�j��1�Ԓn�ł�����p�ɐ��l1�����邱�ƂɂȂ�܂��B

�ȉ��̖��߂͂���܂���B

    mov &j,p ;(NG�j

&j�͐��l1���Ӗ����܂��B���l��1��p���W�X�^�̒l������邱�Ƃ͂ł��܂���B

## ���ߍs
���s���閽�߂���ׂĂ���܂��B
1�s���ҏW�ł��܂��B

## step���s�{�^��
step��������1���߂����s���܂��B

## reset���s�{�^��
reset�������ƍŏ��̖��߂ɖ߂�܂��B

## insert�{�^��
insert�������Ɩ��ߍs�𑝂₷���Ƃ��ł��܂��B

## �C���X�g�[��

    mkdir crypto
    cd crypto
    npm install --save nw

## �v���O�����̎��s

nw.js�Ŏ��s�ł��܂��B

..\node_modules\.bin\nw







CryptoAsm is virtual assembler.

It is an assembler to understand the point of C language.

mov p,1   ; p <- 1.  Register p has  address 1 of memory.
mov a,*p  ; Register a <- Contents of memory address 1.


