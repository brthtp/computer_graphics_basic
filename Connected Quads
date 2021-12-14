#include<GL/glut.h>
int p1[] = { 20, 50 };
int p2[] = { 10, 10 };
int p3[] = { 25, 30 };
int p4[] = { 30, 50 };
int p5[] = { 60, 70 };
int p6[] = { 80, 10 };
int p7[] = { 100, 50 };
int p8[] = { 80, 100 };
void init(void)
{
 glClearColor(0.0, 0.0, 0.0, 1.0);
 glMatrixMode(GL_PROJECTION);
 gluOrtho2D(0.0, 250.0, 0.0, 200.0);
}
void threeconnectedquads(void)
{
 glClear(GL_COLOR_BUFFER_BIT);
 glColor3d(1.0, 1.0, 0.0);
 glBegin(GL_QUAD_STRIP);
 glVertex2iv(p1);
 glVertex2iv(p2);
 glVertex2iv(p4);
 glVertex2iv(p3);
 glVertex2iv(p5);
 glVertex2iv(p6);
 glVertex2iv(p8);
 glVertex2iv(p7);
 glEnd();
 glFlush();
}
int main(int argc, char** argv)
{
 glutInit(&argc, argv);
 glutInitDisplayMode(GLUT_SINGLE | GLUT_RGB);
 glutInitWindowSize(500, 400);
 glutInitWindowPosition(0, 0);
 glutCreateWindow("Three_Connected_Quads");
 init();
 glutDisplayFunc(threeconnectedquads);
 glutMainLoop();
}
