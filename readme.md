qtbase_zh_CN.ts

��֪ʲôԭ�򣬹ٷ�������Qt5.2������qtbaseϵ�е����ķ��롣
�⽫����QMessageBox�İ�ť�޷���������Ϊ�����յ�����QPlatformTheme����غ�������QPlatformTheme��������qt_zh_CN�С�

���к�qt_zh_CN.ts�ظ����ı����Ѿ����루ʹ��TsSync���ߣ���ʣ�µķ�����һ���֣��о������˿��Գ��Զ������ꡣ

usage:
`
int main(int argc, char *argv[])
{
    QApplication app(argc, argv);

    QTranslator qtTranslator;
    qtTranslator.load("qt_zh_CN.qm", QLibraryInfo::location(QLibraryInfo::TranslationsPath));
    app.installTranslator(&qtTranslator);

    QTranslator qtbaseTranslator;
    qtbaseTranslator.load("qtbase_zh.qm");
    app.installTranslator(&qtbaseTranslator);

    ...
    return app.exec();
}
`
