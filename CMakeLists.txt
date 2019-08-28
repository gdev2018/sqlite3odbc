cmake_minimum_required(VERSION 3.14)
project(sqlite3odbc C)

set(CMAKE_C_STANDARD 11)

include_directories(.)
include_directories(missing)

add_executable(sqlite3odbc
        missing/ini.h
        missing/log.h
        tccex/obench.c
        tccex/samplext.c
        tccex/sbench.c
        tccex/sqlite.c
        tccex/sqlite3.c
        adddsn.c
        blobtoxy.c
        csvtable.c
        fixup.c
        impexp.c
        impexp.h
        inst.c
        mkopc.c
        mkopc3.c
        resourceos2.h
        sqlite+tcc.c
        sqlite3odbc.c
        sqlite3odbc.h
        sqlite4odbc.c
        sqlite4odbc.h
        sqliteodbc.c
        sqliteodbc.h
        SQLiteODBCInstaller.c
        xpath.c
        zipfile.c)
