<p><H3>�I�[���E�F�[�u DSP���W�IIC SI4732��Pi Pico�Ő��䂷��</H3></p>
<p>
GitHub�ɂ���SI4732��<a href="https://github.com/pu2clr/SI4735">���C�u����</a>�ɂ́APi Pico��SI4732�𐧌䂷�邱�Ƃ��ł���Ƃ���A"example"�ɗႪ����B<br>
�����ł́A�@�\�I�Ɋ������Ă���Arduino Pro mini�Ή���"SI47XX_02_ALL_IN_ONE_OLED"��Pi Pico�p�ɉ��C������������B<br>
�J����Arduino IDE 2.1�ōs�����B<br>
</p>

<p><strong>�T�v</strong><br>
���C�O�̃X�P�b�`�ł́A������{�^���ƃ��[�^���[�G���R�[�_�[�ōs���Ă���B����́A���̂܂ܕύX���Ȃ����Ƃɂ���BI2C�ƃ��Z�b�g�̃s���͕ύX����B<br>
�Ȃ��A��H�i"schematic2.pdf"�j�Ƃ��ẮASI4732�̃I�[�f�B�I�o�͕s����₤���߂Ɗ��x����̂��߁A�I�y�A���v�̑�����H�i���[�p�X�t�B���^�t�j��<br>
�g�����W�X�^�̍����g������H��ǉ����Ă���B<br>
�����ɂ��Ă͊�iPCB�j�����s�����B<br>
</p>
<p><strong>H/W�\��</strong><br>
 �ERaspberry Pi Pico - �R���g���[��<br>
 �EI2C�ڑ�&nbsp; SI4732<br>
 �EI2C�ڑ�&nbsp; OLED�\�����u(SSD1306)<br>
 �E�{�^���ƃ��[�^���[�G���R�[�_�[<br>
 �E�I�y�A���v NJM4580<br>
 �E�����g���� �g�����W�X�^ S9018<br>
 �EXtal���U��i32768Hz�j�A��R�E�R���f���T�ށA�I�[�f�B�I�W���b�N�A�z����<br>
</p>
<p>
<img src="./SI4732_Pi_Pico_1.jpg" width="480" height="360"><br>
</p>
<p><strong>�ڑ�</strong><br>
�e�R���|�[�l���g�̐ڑ��͈ȉ��̒ʂ�B<br>
<p>
<table> 
<tr>
<td>I2C&nbsp;</td><td>Pi_Pico</td>
</tr>
<tr>
<td>SDA(SI4732,OLED)</td><td>20</td>
</tr>
<tr>
<td>SCK(SI4732,OLED)</td><td>21</td>
</tr>
<tr>
<td>RESET(SI4732)</td><td>22</td>
</tr>
</table>
</p>
*���̑��̐ڑ��ɂ��ẮA�X�P�b�`���Q�Ƃ̂���<br>
**�v���A�b�v��R�͏ȗ���<br>
</p>
<p><strong>�C���X�g�[��</strong><br>
<ol>
<li>�R�[�h���AZIP�`���Ń_�E�����[�h</li>
<li>�ǉ��̃��C�u�������AZIP�`���Ń_�E�����[�h���̓��C�u�����}�l�[�W������C���X�g�[������</li>
 <ul>
  <li>SI4735�i���C�u�����}�l�[�W�����猟���j</li>
  <li>Tiny4kOLED�i���C�u�����}�l�[�W�����猟���j</li>
 </ul>
<li>ArduinoIDE����SI47XX_02_ALL_IN_ONE_OLED_pi_pico_master.ino���J��</li>
<li>�u���؁E�R���p�C���v�ɐ���������A��U�A�u���O��t���ĕۑ��v���s��</li>
</ol>
</p>
<p><strong>�኱�̉��</strong><br>
�ESTEP�̃{�^���i�G���R�[�_�ɐڑ��j�́AFM��M���͎��g���̃v���Z�b�g�i�ϐ�"fmstation[] "�ɒ�`�j�؂�ւ��Ƃ��ē��삷��B<br>
�E�d���������Pi Pico��LED���_������B<br>
�E�ϐ�"Band band[]"�̂S�Ԗڂ̒萔�́A�o���h�؂�ւ����̊���̎�M���g���ł���B�n��̕����ǂɍ��킹��Ɨǂ��B<br>
<p>
<img src="./SI4732_Pi_Pico_2.jpg" width="540" height="360"><br>
</p>
</p>
<p><strong>���ӎ���</strong><br>
�E���p�̍ۂ́A���ȐӔC�ł��y���݂��������B<br>
</p>
