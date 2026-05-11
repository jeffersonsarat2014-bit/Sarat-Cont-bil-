# Criar o projeto Expo
npx create-expo-app ContabilidadePRO
cd ContabilidadePRO

# Instalar as bibliotecas que desenvolvemos
npx expo install @react-navigation/native @react-navigation/stack react-native-screens react-native-safe-area-context react-native-gesture-handler react-native-reanimated react-native-chart-kit react-native-svg expo-image-picker @supabase/supabase-js
Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq
 Command k in package kona
 Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3
 Command lr in package lr
 Command lx in package lux-cli
 Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton
 Command 7z in package p7zip
 Command gp in package pari
 Command pb in package pb
 Command ps in package procps
 Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
~ $ import React, { useState, useEffect } from 'react';
import { View, Text, TextInput, FlatList, StyleSheet } from 'react-native';

function ListaClientesReal() {
  const [busca, setBusca] = useState('');
  const [clientes, setClientes] = useState([
    { id: '1', nome: 'Mercado Silva', status: 'Ativo' },
    { id: '2', nome: 'Auto Peças MT', status: 'Inativo' },
    { id: '3', nome: 'Loja Centro', status: 'Ativo' },
    { id: '4', nome: 'Distribuidora Cuiabá', status: 'Pendente' },
  ]);
  const [clientesFiltrados, setClientesFiltrados] = useState([]);                                               
  // Toda vez que o texto da busca mudar, filtramos a lista
  useEffect(() => {
    const resultado = clientes.filter(cliente =>
      cliente.nome.toLowerCase().includes(busca.toLowerCase())
    );
    setClientesFiltrados(resultado);
  }, [busca, clientes]);

  return (
    <View style={styles.container}>
      {/* CAMPO DE BUSCA */}
      <View style={styles.searchSection}>
        <TextInput
          style={styles.searchInput}
          placeholder="🔍 Buscar cliente por nome..."
          value={busca}
          onChangeText={setBusca}
          placeholderTextColor="#94a3b8"
        />
      </View>

      {/* LISTA FILTRADA */}
      <FlatList
        data={clientesFiltrados}
        keyExtractor={item => item.id}
        renderItem={({ item }) => (
          <View style={styles.listItem}>
            <View>
              <Text style={styles.listText}>{item.nome}</Text>
              <Text style={styles.statusLabel}>{item.status}</Text>
            </View>
            <View style={[styles.statusDot, { backgroundColor: item.status === 'Ativo' ? '#10b981' : '#f59e0b' }]} />
          </View>
        )}
        ListEmptyComponent={
          <Text style={styles.emptyText}>Nenhum cliente encontrado.</Text>
        }
      />
    </View>
  );
}
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `('
bash: //: Is a directory
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `.includes'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `resultado'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `newline'
~ $ const styles = StyleSheet.create({
  container: { flex: 1, backgroundColor: '#f8fafc', padding: 15 },
  searchSection: {
    backgroundColor: '#fff',
    borderRadius: 15,
    paddingHorizontal: 15,
    marginBottom: 20,
    borderWidth: 1,
    borderColor: '#e2e8f0',
    elevation: 2, // Sombra suave no Android
  },
  searchInput: {
    height: 50,                                             fontSize: 16,
    color: '#1e293b',
  },
  listItem: {
    backgroundColor: '#fff',
    padding: 20,
    borderRadius: 18,
    marginBottom: 12,
    flexDirection: 'row',
    justifyContent: 'space-between',
    alignItems: 'center',
    borderWidth: 1,
    borderColor: '#f1f5f9',
  },
  listText: { fontSize: 16, fontWeight: 'bold', color: '#334155' },
  statusLabel: { fontSize: 12, color: '#64748b', marginTop: 4 },
  statusDot: { width: 10, height: 10, borderRadius: 5 },
  emptyText: { textAlign: 'center', color: '#94a3b8', marginTop: 50 }
});
bash: syntax error near unexpected token `('
No command container: found, did you mean:
 Command containerd in package containerd from the root-repo repository
searchSection:: command not found
backgroundColor:: command not found
borderRadius:: command not found
paddingHorizontal:: command not found
marginBottom:: command not found
borderWidth:: command not found
borderColor:: command not found
elevation:: command not found
No command }, found, did you mean:
 Command ab in package apache2
 Command at in package at
 Command bc in package bc
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command nc in package busybox
 Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups
 Command d8 in package d8
 Command sh in package dash
 Command dx in package dx
 Command ed in package ed
 Command ef in package electric-fence
 Command et in package et
 Command fd in package fd
 Command fm in package fm
 Command fx in package fx
 Command dl in package gatling
 Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq
 Command k in package kona
 Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3
 Command lr in package lr
 Command lx in package lux-cli
 Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton
 Command 7z in package p7zip
 Command gp in package pari
 Command pb in package pb
 Command ps in package procps
 Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command st in package st from the x11-repo repository
 Command sr in package surfraw
 Command pt in package tcllib
 Command am in package termux-am
 Command df in package termux-tools
 Command ht in package texlive-bin
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command ug in package ugrep
 Command up in package up
 Command ul in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command wg in package wireguard-tools
 Command xh in package xh
 Command X in package xorg-server from the x11-repo repository
 Command xz in package xz-utils
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zk in package zk
searchInput:: command not found
height:: command not found
fontSize:: command not found
No command color: found, did you mean:
 Command colorit in package dictd
 Command colcrt in package util-linux
No command }, found, did you mean:
 Command ab in package apache2
 Command at in package at
 Command bc in package bc
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command nc in package busybox
 Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups
 Command d8 in package d8
 Command sh in package dash
 Command dx in package dx
 Command ed in package ed
 Command ef in package electric-fence
 Command et in package et
 Command fd in package fd
 Command fm in package fm
 Command fx in package fx
 Command dl in package gatling
 Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq
 Command k in package kona
 Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3
 Command lr in package lr
 Command lx in package lux-cli
 Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton
 Command 7z in package p7zip
 Command gp in package pari
 Command pb in package pb
 Command ps in package procps
 Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command st in package st from the x11-repo repository
 Command sr in package surfraw
 Command pt in package tcllib
 Command am in package termux-am
 Command df in package termux-tools
 Command ht in package texlive-bin
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command ug in package ugrep
 Command up in package up
 Command ul in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command wg in package wireguard-tools
 Command xh in package xh
 Command X in package xorg-server from the x11-repo repository
 Command xz in package xz-utils
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zk in package zk
listItem:: command not found
backgroundColor:: command not found
padding:: command not found
borderRadius:: command not found
marginBottom:: command not found
flexDirection:: command not found
justifyContent:: command not found
alignItems:: command not found
borderWidth:: command not found
borderColor:: command not found
No command }, found, did you mean:
 Command ab in package apache2
 Command at in package at
 Command bc in package bc
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command nc in package busybox
 Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups
 Command d8 in package d8
 Command sh in package dash
 Command dx in package dx
 Command ed in package ed
 Command ef in package electric-fence
 Command et in package et
 Command fd in package fd
 Command fm in package fm
 Command fx in package fx
 Command dl in package gatling
 Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq
 Command k in package kona
 Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3
 Command lr in package lr
 Command lx in package lux-cli
 Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton
 Command 7z in package p7zip
 Command gp in package pari
 Command pb in package pb
 Command ps in package procps
 Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command st in package st from the x11-repo repository
 Command sr in package surfraw
 Command pt in package tcllib
 Command am in package termux-am
 Command df in package termux-tools
 Command ht in package texlive-bin
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command ug in package ugrep
 Command up in package up
 Command ul in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command wg in package wireguard-tools
 Command xh in package xh
 Command X in package xorg-server from the x11-repo repository
 Command xz in package xz-utils
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zk in package zk
listText:: command not found
statusLabel:: command not found
statusDot:: command not found
emptyText:: command not found
bash: syntax error near unexpected token `}'
~ $ {
  "expo": {
    "name": "Contabilidade PRO",
    "slug": "contabilidade-pro",
    "version": "1.0.0",
    "orientation": "portrait",
    "icon": "./assets/icon.png",
    "android": {
      "package": "com.seuusuario.contabilidadepro", // ID Único no mundo
      "adaptiveIcon": {
        "foregroundImage": "./assets/adaptive-icon.png",
        "backgroundColor": "#1d4ed8"
      }
    }
  }
}
No command expo: found, did you mean:
 Command expr in package coreutils
No command name: found, did you mean:
 Command named in package dnsutils
 Command namei in package util-linux
No command slug: found, did you mean:
 Command blogc in package blogc
 Command shuf in package coreutils
 Command fluid in package fltk from the x11-repo repository
 Command glue in package gluelang
 Command gnugo in package gnugo
 Command hugo in package hugo
 Command lego in package lego
 Command lua in package lua51
 Command lua in package lua52
 Command lua in package lua53
 Command lua in package lua54
 Command lua in package lua55
 Command luvi in package luvi
 Command lux in package lux
 Command pluma in package pluma from the x11-repo repository
 Command pluto in package plutolang
 Command pslog in package psmisc
 Command rlog in package rcs
 Command svlogd in package runit
 Command sl in package sl
 Command slsh in package slang
 Command slugify in package slugify
 Command squid in package squid
 Command stag in package stag
~ $ import React, { useState } from 'react';
import { View, Text, TouchableOpacity, Image, StyleSheet, Alert } from 'react-native';
import * as ImagePicker from 'expo-image-picker';
import { supabase } from './supabase'; // Sua conexão

export default function EnviarDocumento() {
  const [image, setImage] = useState(null);
  const [uploading, setUploading] = useState(false);    
  // 1. Pedir permissão e abrir a câmera
  const tirarFoto = async () => {
    const { status } = await ImagePicker.requestCameraPermissionsAsync();

    if (status !== 'granted') {
      Alert.alert("Permissão necessária", "Precisamos de acesso à câmera para escanear a nota.");
      return;
    }

    let result = await ImagePicker.launchCameraAsync({
      allowsEditing: true, // Permite cortar a foto da nota
      quality: 0.7,        // Reduz o peso do arquivo para economizar internet
    });
                                                            if (!result.canceled) {
      setImage(result.assets[0].uri);
    }
  };

  // 2. Enviar para o Storage do Supabase (Nuvem)
  const enviarParaContador = async () => {
    if (!image) return;
    setUploading(true);

    try {
      const fileName = `nota_${Date.now()}.jpg`;
      const formData = new FormData();
      formData.append('file', {
        uri: image,
        name: fileName,
        type: 'image/jpeg',
      });

      // Aqui você faria o upload para o bucket 'documentos' do Supabase
      const { error } = await supabase.storage
        .from('documentos')
        .upload(fileName, formData);

      if (error) throw error;

      Alert.alert("Sucesso!", "Documento enviado para análise do contador.");
      setImage(null);
    } catch (error) {
      Alert.alert("Erro no envio", error.message);
    } finally {
      setUploading(false);
    }
  };

  return (
    <View style={styles.container}>
      <Text style={styles.title}>Escanear Documento</Text>

      <TouchableOpacity style={styles.cameraBtn} onPress={tirarFoto}>
        <Text style={styles.btnText}>📸 Tirar Foto da Nota</Text>
      </TouchableOpacity>

      {image && (
        <View style={styles.previewContainer}>
          <Image source={{ uri: image }} style={styles.preview} />
          <TouchableOpacity
            style={[styles.sendBtn, uploading && {backgroundColor: '#94a3b8'}]}
            onPress={enviarParaContador}
            disabled={uploading}
          >
            <Text style={styles.btnText}>{uploading ? "Enviando..." : "Confirmar e Enviar"}</Text>
          </TouchableOpacity>
        </View>
      )}
    </View>
  );
}

const styles = StyleSheet.create({
  container: { flex: 1, padding: 20, alignItems: 'center', justifyContent: 'center' },
  title: { fontSize: 22, fontWeight: 'bold', marginBottom: 20 },
  cameraBtn: { backgroundColor: '#1d4ed8', padding: 20, borderRadius: 15, width: '100%' },
  sendBtn: { backgroundColor: '#059669', padding: 20, borderRadius: 15, width: '100%', marginTop: 20 },
  btnText: { color: '#fff', textAlign: 'center', fontWeight: 'bold' },
  preview: { width: 300, height: 400, borderRadius: 10, marginTop: 20 },
  previewContainer: { width: '100%', alignItems: 'center' }
});                                                     The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:                                                    pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
bash: //: Is a directory
bash: syntax error near unexpected token `('            bash: syntax error near unexpected token `('            bash: syntax error near unexpected token `('
bash: //: Is a directory                                bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `{'
bash: syntax error near unexpected token `"Permissão necessária",'                                              bash: return: can only `return' from a function or sourced script                                               bash: syntax error near unexpected token `}'            bash: syntax error near unexpected token `('            allowsEditing:: command not found                       quality:: command not found
bash: syntax error near unexpected token `}'            bash: !result.canceled: event not found                 bash: syntax error near unexpected token `result.assets[0].uri'
bash: syntax error near unexpected token `}'            bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: !image: event not found
bash: syntax error near unexpected token `true'         No command try found, did you mean:                      Command tr in package coreutils                         Command tri in package mesa-demos from the x11-repo repository
 Command trz in package trzsz-go                        bash: nota_${Date.now()}.jpg: bad substitution          No command const found, did you mean:
 Command cpnt in package chntpw
 Command ctest in package cmake                          Command host in package dnsutils                        Command dunst in package dunst from the x11-repo repository                                                     Command gost in package gost
 Command count in package llvm-tools
 Command most in package most
 Command chpst in package runit
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `'file','      No command uri: found, did you mean:
 Command uniq in package coreutils
 Command tri in package mesa-demos from the x11-repo repository                                                  Command uuid in package ossp-uuid
 Command uic in package qt5-qtbase from the x11-repo repository
 Command rig in package rig
 Command rip in package rip2
 Command ri in package ruby-ri
No command name: found, did you mean:
 Command named in package dnsutils
 Command namei in package util-linux
No command type: found, did you mean:
 Command typer in package erlang
bash: syntax error near unexpected token `}'
bash: //: Is a directory
No command const found, did you mean:
 Command cpnt in package chntpw                          Command ctest in package cmake
 Command host in package dnsutils
 Command dunst in package dunst from the x11-repo repository
 Command gost in package gost                            Command count in package llvm-tools
 Command most in package most
 Command chpst in package runit                         bash: syntax error near unexpected token `'documentos''
bash: syntax error near unexpected token `fileName,'    bash: syntax error near unexpected token `throw'
bash: syntax error near unexpected token `"Sucesso!",'
bash: syntax error near unexpected token `null'
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `"Erro no envio",'
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `false'
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: TouchableOpacity: No such file or directory
uploading: command not found
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'            bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'            bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `('
No command container: found, did you mean:               Command containerd in package containerd from the root-repo repository
No command title: found, did you mean:
 Command bitlbee in package bitlbee
 Command figlet in package figlet
 Command file in package file
 Command gitea in package gitea
~ $ import { Dimensions } from 'react-native';          import { LineChart } from 'react-native-chart-kit';
                                                        const screenWidth = Dimensions.get("window").width;
                                                        function FinanceChart() {
  return (                                                  <View style={styles.chartContainer}>
      <Text style={styles.sectionTitle}>Evolução de Receitas</Text>                                                   <LineChart
        data={{
          labels: ["Jan", "Fev", "Mar", "Abr", "Mai", "Jun"],
          datasets: [
            {
              data: [45, 52, 48, 70, 86, 92], // Valores em mil reais
              color: (opacity = 1) => `rgba(29, 78, 216, ${opacity})`, // Azul PRO
              strokeWidth: 3                                        }
          ]                                                     }}
        width={screenWidth - 30} // Largura da tela menos o padding
        height={220}
        chartConfig={{                                            backgroundColor: "#fff",                                backgroundGradientFrom: "#fff",
          backgroundGradientTo: "#fff",                           decimalPlaces: 0,
          color: (opacity = 1) => `rgba(30, 41, 59, ${opacity})`,
          labelColor: (opacity = 1) => `rgba(100, 116, 139, ${opacity})`,
          style: { borderRadius: 16 },                            propsForDots: {
            r: "6",
            strokeWidth: "2",
            stroke: "#1d4ed8"                                     }
        }}                                                      bezier // Suaviza a linha do gráfico                    style={{
          marginVertical: 8,                                      borderRadius: 16
        }}
      />                                                    </View>                                               );                                                    }                                                       The program import is not installed. Install it by executing:
 pkg install imagemagick                                The program import is not installed. Install it by executing:
 pkg install imagemagick
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: LineChart: No such file or directory
No command labels: found, did you mean:                  Command abcls in package alembic
 Command mlabel in package mtools                       datasets:: command not found
bash: syntax error near unexpected token `opacity'      strokeWidth:: command not found
bash: syntax error near unexpected token `}'
No command ] found, did you mean:
 Command [ in package coreutils
 Command k in package kona
 Command o in package orbiton
 Command q in package q-dns-client
 Command X in package xorg-server from the x11-repo repository
No command }} found, did you mean:
 Command ab in package apache2                           Command at in package at
 Command bc in package bc
 Command ar in package binutils
 Command as in package binutils-bin                      Command ar in package binutils-is-llvm
 Command bk in package bk                                Command nc in package busybox
 Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups
 Command d8 in package d8
 Command sh in package dash                              Command dx in package dx
 Command ed in package ed
 Command ef in package electric-fence
 Command et in package et                                Command fd in package fd
 Command fm in package fm                                Command fx in package fx
 Command dl in package gatling
 Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository   Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo                                Command jq in package jq
 Command k in package kona                               Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3                        Command lr in package lr
 Command lx in package lux-cli                           Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils                         Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton
 Command 7z in package p7zip                             Command gp in package pari
 Command pb in package pb                                Command ps in package procps
 Command pd in package proot-distro                      Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2                           Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
 Command ag in package silversearcher-ag
 Command sl in package sl                                Command st in package st from the x11-repo repository
 Command sr in package surfraw                           Command pt in package tcllib
 Command am in package termux-am                         Command df in package termux-tools
 Command ht in package texlive-bin                       Command sn in package tin-summer
 Command tf in package tinyfugue
 Command ug in package ugrep
 Command up in package up
 Command ul in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis                               Command wg in package wireguard-tools
 Command xh in package xh                                Command X in package xorg-server from the x11-repo repository
 Command xz in package xz-utils
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3                                Command zk in package zk
No command - found, did you mean:                        Command [ in package coreutils
 Command k in package kona                               Command o in package orbiton
 Command q in package q-dns-client                       Command X in package xorg-server from the x11-repo repository                                                  backgroundColor:: command not found
backgroundGradientFrom:: command not found
backgroundGradientTo:: command not found
decimalPlaces:: command not found                       bash: syntax error near unexpected token `opacity'
bash: syntax error near unexpected token `opacity'      No command style: found, did you mean:                   Command stylua in package stylua
propsForDots:: command not found                        No command r: found, did you mean:
 Command rm in package coreutils
 Command r8 in package d8                                Command r2 in package radare2
 Command rc in package rc                                Command rg in package ripgrep                           Command rq in package rq
 Command ri in package ruby-ri
 Command rw in package rw                               strokeWidth:: command not found
No command stroke: found, did you mean:
 Command stoken in package stoken                       bash: syntax error near unexpected token `}'
No command }} found, did you mean:
 Command ab in package apache2                           Command at in package at
 Command bc in package bc
 Command ar in package binutils                          Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk                                Command nc in package busybox
 Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups
 Command d8 in package d8
 Command sh in package dash                              Command dx in package dx
 Command ed in package ed
 Command ef in package electric-fence
 Command et in package et                                Command fd in package fd
 Command fm in package fm
 Command fx in package fx                                Command dl in package gatling
 Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq
 Command k in package kona
 Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3
 Command lr in package lr
 Command lx in package lux-cli
 Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton
 Command 7z in package p7zip
 Command gp in package pari
 Command pb in package pb
 Command ps in package procps
 Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command st in package st from the x11-repo repository
 Command sr in package surfraw
 Command pt in package tcllib
 Command am in package termux-am
 Command df in package termux-tools
 Command ht in package texlive-bin
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command ug in package ugrep
 Command up in package up
 Command ul in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command wg in package wireguard-tools
 Command xh in package xh
 Command X in package xorg-server from the x11-repo repository
 Command xz in package xz-utils
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zk in package zk
The program bezier is not installed. Install it by executing:
 pkg install mesa-demos, after running pkg install x11-repo
marginVertical:: command not found
borderRadius:: command not found
No command }} found, did you mean:
 Command ab in package apache2
 Command at in package at
 Command bc in package bc
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command nc in package busybox                           Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups                              Command d8 in package d8
 Command sh in package dash
 Command dx in package dx
 Command ed in package ed
 Command ef in package electric-fence
 Command et in package et
 Command fd in package fd
 Command fm in package fm
 Command fx in package fx
 Command dl in package gatling
 Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq
 Command k in package kona
 Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3
 Command lr in package lr
 Command lx in package lux-cli
 Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg                                Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc                       Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton                            Command 7z in package p7zip
 Command gp in package pari                              Command pb in package pb
 Command ps in package procps                            Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command st in package st from the x11-repo repository
 Command sr in package surfraw
 Command pt in package tcllib
 Command am in package termux-am
 Command df in package termux-tools
 Command ht in package texlive-bin
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command ug in package ugrep
 Command up in package up
 Command ul in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command wg in package wireguard-tools
 Command xh in package xh
 Command X in package xorg-server from the x11-repo repository
 Command xz in package xz-utils
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zk in package zk
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `}'
~ $   chartContainer: {
    backgroundColor: '#fff',
    margin: 15,
    padding: 15,
    borderRadius: 25,
    elevation: 3,
    shadowColor: '#000',
    shadowOpacity: 0.1,
    shadowRadius: 10,
  },
chartContainer:: command not found                      backgroundColor:: command not found
No command margin: found, did you mean:
 Command argon2 in package argon2
 Command magick in package imagemagick
padding:: command not found
borderRadius:: command not found
elevation:: command not found
shadowColor:: command not found
shadowOpacity:: command not found
shadowRadius:: command not found
No command }, found, did you mean:
 Command ab in package apache2
 Command at in package at
 Command bc in package bc                                Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command nc in package busybox
 Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups
 Command d8 in package d8                                Command sh in package dash
 Command dx in package dx
 Command ed in package ed
 Command ef in package electric-fence
 Command et in package et
 Command fd in package fd
 Command fm in package fm
 Command fx in package fx
 Command dl in package gatling                           Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq                                Command k in package kona
 Command lf in package lf
 Command pl in package libgnustep-base
 Command h3 in package libuber-h3                        Command lr in package lr
 Command lx in package lux-cli
 Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton                            Command 7z in package p7zip
 Command gp in package pari
 Command pb in package pb
 Command ps in package procps
 Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw                               ~ $ import React, { useState } from 'react';
import { View, Text, TouchableOpacity, StyleSheet, Clipboard, Alert } from 'react-native';

export default function PagamentoScreen() {
  // Em um cenário real, esse código viria da API do seu banco (Asaas, Mercado Pago, etc.)
  const [codigoPix, setCodigoPix] = useState('00020126580014BR.GOV.BCB.PIX013663a8a3a3-a3a3-a3a3-a3a3-a3a3a3a3a3a35204000053039865405199.005802BR5925NOME_DO_SEU_APP6009CUIABA62070503***6304ABCD');

  const copiarPix = () => {                                 Clipboard.setString(codigoPix);
    Alert.alert(
      "Código Copiado!",
      "Agora abra o app do seu banco e escolha a opção 'PIX Copia e Cola' para finalizar o pagamento.",               [{ text: "OK" }]
    );
  };

  return (
    <View style={styles.payContainer}>                        <Text style={styles.payTitle}>Assinatura Mensal</Text>
      <View style={styles.valueCard}>
        <Text style={styles.valueLabel}>Valor a pagar:</Text>
        <Text style={styles.valueText}>R$ 199,00</Text>
      </View>
                                                              <View style={styles.pixBox}>
        <Text style={styles.pixInstruction}>
          Clique no botão abaixo para copiar o código PIX:
        </Text>

        <TouchableOpacity style={styles.copyButton} onPress={copiarPix}>
          <Text style={styles.copyButtonText}>📋 Copiar Código PIX</Text>
        </TouchableOpacity>
      </View>

      <Text style={styles.footerNote}>
        A liberação do sistema é imediata após a confirmação.
      </Text>
    </View>
  );
}
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `codigoPix'
bash: syntax error near unexpected token `newline'
Código Copiado!,: command not found
Agora abra o app do seu banco e escolha a opção 'PIX Copia e Cola' para finalizar o pagamento.,: command not found
No command [{ found, did you mean:
 Command [ in package coreutils
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
No command Clique found, did you mean:
 Command clidle in package clidle
 Command glue in package gluelang
 Command lite in package litespeedtest
 Command loqui in package loqui from the x11-repo repository
 Command line in package mesa-demos from the x11-repo repository
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
No command A found, did you mean:
 Command [ in package coreutils
 Command k in package kona
 Command o in package orbiton
 Command q in package q-dns-client
 Command X in package xorg-server from the x11-repo repository
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `}'
~ $ const styles = StyleSheet.create({
  payContainer: { flex: 1, padding: 25, backgroundColor: '#f8fafc', justifyContent: 'center' },
  payTitle: { fontSize: 24, fontWeight: 'bold', textAlign: 'center', color: '#1e293b', marginBottom: 30 },        valueCard: { backgroundColor: '#fff', padding: 25, borderRadius: 20, alignItems: 'center', elevation: 2, marginBottom: 30 },
  valueLabel: { color: '#64748b', fontSize: 16 },
  valueText: { fontSize: 36, fontWeight: '900', color: '#1d4ed8', marginTop: 5 },
  pixBox: { backgroundColor: '#eff6ff', padding: 20, borderRadius: 20, borderStyle: 'dashed', borderWidth: 2, borderColor: '#1d4ed8' },
  pixInstruction: { textAlign: 'center', color: '#1e3a8a', marginBottom: 15, fontSize: 14 },
  copyButton: { backgroundColor: '#1d4ed8', padding: 15, borderRadius: 12, alignItems: 'center' },
  copyButtonText: { color: '#fff', fontWeight: 'bold' },
  footerNote: { textAlign: 'center', color: '#94a3b8', fontSize: 12, marginTop: 20 }
});
bash: syntax error near unexpected token `('
payContainer:: command not found
payTitle:: command not found
valueCard:: command not found
valueLabel:: command not found
valueText:: command not found
pixBox:: command not found
pixInstruction:: command not found
copyButton:: command not found
copyButtonText:: command not found
footerNote:: command not found
bash: syntax error near unexpected token `}'
~ $ /contabilidade-pro
├── src/
│   ├── assets/          # Imagens, ícones e logos
│   ├── components/      # Componentes reutilizáveis (Botões, Cards, Inputs)                                    │   ├── services/        # Configuração do Supabase, APIs e Pagamentos
│   ├── screens/         # As telas completas (Login, Home, Cadastro, Pix)
│   ├── navigation/      # Configuração das rotas (Stack, Tabs)                                                 │   └── styles/          # Temas de cores e estilos globais
├── App.js               # Ponto de entrada que apenas chama o Navigator
└── app.json             # Configurações do Expo/Lojas
bash: /contabilidade-pro: No such file or directory
├──: command not found
No command │ found, did you mean:
 Command 7zz in package 7zip
 Command ack in package ack-grep
 Command acr in package acr
 Command age in package age
 Command agg in package agg
 Command aha in package aha
 Command adb in package android-tools
 Command ant in package ant
 Command ab in package apache2
 Command apt in package apt
 Command arj in package arj
 Command ark in package ark from the x11-repo repository
 Command a2x in package asciidoc
 Command asy in package asymptote
 Command at in package at
 Command als in package atool                            Command aws in package awscli
 Command bat in package bat
 Command bc in package bc                                Command bsh in package beanshell
 Command bed in package bed
 Command ar in package binutils                          Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command atc in package bsd-games                        Command buf in package buf
 Command ash in package busybox
 Command bvi in package bvi
 Command cfm in package cfm                              Command cjs in package cjs from the x11-repo repository
 Command c++ in package clang
 Command ccr in package codecrypt
 Command cbc in package coinor-cbc
 Command clp in package coinor-clp
 Command ctr in package containerd from the root-repo repository
 Command [ in package coreutils
 Command ocs in package cscope                           Command lp in package cups
 Command cvs in package cvs
 Command d8 in package d8
 Command dar in package dar                              Command sh in package dash
 Command dlv in package delve
 Command dia in package dia from the x11-repo repository
 Command cmp in package diffutils
 Command bzz in package djvulibre                        Command dig in package dnsutils                         Command scp in package dropbear
 Command dtc in package dtc
 Command dte in package dte                              Command dua in package dua
 Command duc in package duc
 Command duf in package duf
 Command duk in package duktape                          Command dwm in package dwm from the x11-repo repository
 Command dx in package dx
 Command e16 in package e16 from the x11-repo repository
 Command ecj in package ecj
 Command ecl in package ecl                              Command ed in package ed
 Command eja in package eja
 Command ef in package electric-fence                    Command iex in package elixir
 Command eog in package eog from the x11-repo repository
 Command eom in package eom from the x11-repo repository
 Command erl in package erlang
 Command et in package et
 Command tsh in package etsh
 Command eww in package eww from the x11-repo repository
 Command eza in package eza
 Command fcp in package fcp
 Command fd in package fd
 Command fdm in package fdm
 Command feh in package feh from the x11-repo repository
 Command fff in package fff
 Command fio in package fio from the root-repo repository
 Command bbc in package flang
 Command fm in package fm
 Command fx in package fx
 Command fzf in package fzf
 Command fzy in package fzy
 Command gac in package gap                              Command dl in package gatling
 Command awk in package gawk                             Command gbt in package gbt
 Command gdb in package gdb
 Command gdl in package gdrive-downloader
 Command gdu in package gdu                              Command era in package geth-utils
 Command gh in package gh
 Command ghc in package ghc
 Command gs in package ghostscript
 Command git in package git                              Command ein in package gitoxide
 Command gio in package glib
 Command gn in package gn
 Command gpg in package gnupg
 Command go in package golang
 Command tsc in package gotify
 Command gm in package graphicsmagick
 Command dot in package graphviz
 Command eqn in package groff                            Command gsf in package gsf-tools
 Command gum in package gum
 Command gw in package gw from the x11-repo repository   Command ghb in package handbrake from the x11-repo repository
 Command hx in package helix
 Command hcd in package hfsutils                         Command hh in package hstr
 Command hub in package hub
 Command hut in package hut
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command iat in package iat
 Command ftp in package inetutils
 Command ip in package iproute2
 Command na6 in package ipv6toolkit
 Command vvp in package iverilog
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command joe in package joe
 Command jq in package jq
 Command jql in package jql
 Command joe in package jupp
 Command jwm in package jwm from the x11-repo repository
 Command k9s in package k9s
 Command kak in package kakoune
 Command k in package kona                               Command ksu in package krb5
 Command dub in package ldc
 Command ldd in package ldd
 Command lf in package lf
 Command lha in package lhasa
 Command pl in package libgnustep-base
 Command psl in package libpsl
 Command h3 in package libuber-h3
 Command cvt in package libxcvt from the x11-repo repository
 Command lit in package lit
 Command lld in package lld
 Command llc in package llvm
 Command not in package llvm-tools                       Command lnd in package lnd
 Command ksh in package loksh
 Command lr in package lr
 Command lrb in package lrzsz
 Command lsd in package lsd
 Command lua in package lua51
 Command lua in package lua52
 Command lua in package lua53
 Command lua in package lua54
 Command lua in package lua55
 Command lux in package lux
 Command lx in package lux-cli
 Command lvm in package lvm2 from the root-repo repository
 Command lyx in package lyx from the x11-repo repository Command lz4 in package lz4
 Command m4 in package m4
 Command ali in package mailutils
 Command man in package mandoc
 Command mvn in package maven
 Command mc in package mc                                Command mdp in package mdp
 Command mdb in package mercury
 Command ray in package mesa-demos from the x11-repo repository
 Command mg in package mg
 Command mlr in package miller
 Command al in package mono
 Command mop in package mop
 Command pee in package moreutils
 Command mpc in package mpc
 Command mpd in package mpd
 Command mpv in package mpv                              Command mpv in package mpv-x from the x11-repo repository
 Command lz in package mtools
 Command mtr in package mtr from the root-repo repository
 Command mu in package mu
 Command mr in package myrepos                           Command psc in package n-t-roff-sc
 Command tic in package ncurses-utils
 Command ne in package ne
 Command ex in package neovim-nightly,neovim             Command arp in package net-tools
 Command nc in package netcat-openbsd                    Command nim in package nim
 Command nc in package nmap
 Command ali in package nmh
 Command nnn in package nnn
 Command nms in package no-more-secrets                  Command npm in package npm
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command oma in package oma
 Command iv in package openimageio from the x11-repo repository
 Command jar in package openjdk-21                       Command jar in package openjdk-25
 Command scp in package openssh
 Command o in package orbiton
 Command 7z in package p7zip
 Command sem in package parallel
 Command gp in package pari
 Command fpp in package pathpicker
 Command pb in package pb
 Command pet in package pet
 Command php in package php
 Command pil in package picolisp
 Command ode in package plotutils from the x11-repo repository
 Command ps in package procps
 Command cct in package proj
 Command pd in package proot-distro
 Command pup in package pup
 Command pv in package pv
 Command pip in package python-pip
 Command q in package q-dns-client
 Command moc in package qt5-qtbase from the x11-repo repository
 Command qml in package qt5-qtdeclarative from the x11-repo repository
 Command qev in package qt5-qttools from the x11-repo repository
 Command qjs in package quickjs
 Command r2 in package radare2
 Command rbw in package rbw
 Command rc in package rc
 Command ci in package rcs
 Command rem in package remind
 Command icp in package renameutils
 Command rig in package rig
 Command rip in package rip2
 Command rg in package ripgrep
 Command rga in package ripgrep-all
 Command rnr in package rnr
 Command rpm in package rpm
 Command rq in package rq
 Command erb in package ruby
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command net in package samba
 Command scc in package scc
 Command sd in package sd
 Command srm in package secure-delete
 Command sed in package sed
 Command shc in package shc
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command fls in package sleuthkit
 Command gst in package smalltalk
 Command rec in package sox
 Command st in package st from the x11-repo repository
 Command svn in package subversion
 Command sun in package sun
 Command sr in package surfraw
 Command tar in package tar
 Command tsp in package task-spooler
 Command tcc in package tcc
 Command nns in package tcllib
 Command tdl in package tdl
 Command tea in package tea                              Command tsh in package teleport-tsh
 Command am in package termux-am
 Command cmd in package termux-tools                     Command ebb in package texlive-bin
 Command tig in package tig
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command tor in package tor
 Command trz in package trzsz-go
 Command tsu in package tsu
 Command tut in package tut
 Command tjs in package txikijs
 Command ug in package ugrep
 Command up in package up
 Command upx in package upx
 Command cal in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command viu in package viu
 Command vlc in package vlc
 Command vlc in package vlc-qt from the x11-repo repository
 Command vtm in package vtm
 Command w3m in package w3m
 Command wg in package wireguard-tools
 Command wiz in package wiz
 Command wol in package wol
 Command wrk in package wrk
 Command x2x in package x2x from the x11-repo repository
 Command xh in package xh
 Command xml in package xmlstarlet
 Command X in package xorg-server from the x11-repo repository                                                   Command twm in package xorg-twm from the x11-repo repository
 Command xev in package xorg-xev from the x11-repo repository
 Command xxd in package xxd
 Command xz in package xz-utils                          Command yad in package yad from the x11-repo repository
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zip in package zip
 Command zk in package zk
 Command znc in package znc
 Command zsh in package zsh
No command │ found, did you mean:                        Command 7zz in package 7zip
 Command ack in package ack-grep                         Command acr in package acr                              Command age in package age
 Command agg in package agg
 Command aha in package aha                              Command adb in package android-tools                    Command ant in package ant
 Command ab in package apache2
 Command apt in package apt
 Command arj in package arj
 Command ark in package ark from the x11-repo repository
 Command a2x in package asciidoc
 Command asy in package asymptote
 Command at in package at
 Command als in package atool
 Command aws in package awscli
 Command bat in package bat
 Command bc in package bc                                Command bsh in package beanshell
 Command bed in package bed                              Command ar in package binutils
 Command as in package binutils-bin                      Command ar in package binutils-is-llvm
 Command bk in package bk
 Command atc in package bsd-games                        Command buf in package buf
 Command ash in package busybox
 Command bvi in package bvi
 Command cfm in package cfm
 Command cjs in package cjs from the x11-repo repository
 Command c++ in package clang
 Command ccr in package codecrypt
 Command cbc in package coinor-cbc
 Command clp in package coinor-clp
 Command ctr in package containerd from the root-repo repository                                                 Command [ in package coreutils
 Command ocs in package cscope
 Command lp in package cups                              Command cvs in package cvs
 Command d8 in package d8
 Command dar in package dar                              Command sh in package dash
 Command dlv in package delve
 Command dia in package dia from the x11-repo repository
 Command cmp in package diffutils
 Command bzz in package djvulibre
 Command dig in package dnsutils
 Command scp in package dropbear
 Command dtc in package dtc
 Command dte in package dte
 Command dua in package dua
 Command duc in package duc
 Command duf in package duf
 Command duk in package duktape
 Command dwm in package dwm from the x11-repo repository
 Command dx in package dx
 Command e16 in package e16 from the x11-repo repository
 Command ecj in package ecj
 Command ecl in package ecl
 Command ed in package ed
 Command eja in package eja
 Command ef in package electric-fence
 Command iex in package elixir
 Command eog in package eog from the x11-repo repository
 Command eom in package eom from the x11-repo repository
 Command erl in package erlang
 Command et in package et
 Command tsh in package etsh
 Command eww in package eww from the x11-repo repository
 Command eza in package eza
 Command fcp in package fcp
 Command fd in package fd
 Command fdm in package fdm
 Command feh in package feh from the x11-repo repository
 Command fff in package fff
 Command fio in package fio from the root-repo repository
 Command bbc in package flang
 Command fm in package fm
 Command fx in package fx
 Command fzf in package fzf
 Command fzy in package fzy
 Command gac in package gap
 Command dl in package gatling
 Command awk in package gawk
 Command gbt in package gbt
 Command gdb in package gdb
 Command gdl in package gdrive-downloader
 Command gdu in package gdu
 Command era in package geth-utils
 Command gh in package gh
 Command ghc in package ghc
 Command gs in package ghostscript
 Command git in package git
 Command ein in package gitoxide
 Command gio in package glib
 Command gn in package gn
 Command gpg in package gnupg
 Command go in package golang
 Command tsc in package gotify
 Command gm in package graphicsmagick
 Command dot in package graphviz
 Command eqn in package groff
 Command gsf in package gsf-tools
 Command gum in package gum
 Command gw in package gw from the x11-repo repository
 Command ghb in package handbrake from the x11-repo repository
 Command hx in package helix
 Command hcd in package hfsutils
 Command hh in package hstr
 Command hub in package hub
 Command hut in package hut
 Command hz in package hz                                Command i3 in package i3 from the x11-repo repository
 Command iat in package iat
 Command ftp in package inetutils                        Command ip in package iproute2
 Command na6 in package ipv6toolkit
 Command vvp in package iverilog
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command joe in package joe
 Command jq in package jq
 Command jql in package jql
 Command joe in package jupp
 Command jwm in package jwm from the x11-repo repository
 Command k9s in package k9s
 Command kak in package kakoune
 Command k in package kona
 Command ksu in package krb5
 Command dub in package ldc
 Command ldd in package ldd
 Command lf in package lf
 Command lha in package lhasa
 Command pl in package libgnustep-base
 Command psl in package libpsl
 Command h3 in package libuber-h3
 Command cvt in package libxcvt from the x11-repo repository
 Command lit in package lit
 Command lld in package lld
 Command llc in package llvm
 Command not in package llvm-tools
 Command lnd in package lnd
 Command ksh in package loksh
 Command lr in package lr
 Command lrb in package lrzsz
 Command lsd in package lsd
 Command lua in package lua51
 Command lua in package lua52
 Command lua in package lua53                            Command lua in package lua54
 Command lua in package lua55
 Command lux in package lux
 Command lx in package lux-cli
 Command lvm in package lvm2 from the root-repo repository                                                       Command lyx in package lyx from the x11-repo repository
 Command lz4 in package lz4
 Command m4 in package m4
 Command ali in package mailutils
 Command man in package mandoc
 Command mvn in package maven
 Command mc in package mc
 Command mdp in package mdp
 Command mdb in package mercury
 Command ray in package mesa-demos from the x11-repo repository
 Command mg in package mg
 Command mlr in package miller
 Command al in package mono                              Command mop in package mop
 Command pee in package moreutils
 Command mpc in package mpc
 Command mpd in package mpd
 Command mpv in package mpv
 Command mpv in package mpv-x from the x11-repo repository
 Command lz in package mtools
 Command mtr in package mtr from the root-repo repository
 Command mu in package mu
 Command mr in package myrepos
 Command psc in package n-t-roff-sc
 Command tic in package ncurses-utils
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command arp in package net-tools
 Command nc in package netcat-openbsd
 Command nim in package nim
 Command nc in package nmap
 Command ali in package nmh
 Command nnn in package nnn
 Command nms in package no-more-secrets                  Command npm in package npm
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol                                Command oma in package oma
 Command iv in package openimageio from the x11-repo repository                                                  Command jar in package openjdk-21
 Command jar in package openjdk-25
 Command scp in package openssh
 Command o in package orbiton                            Command 7z in package p7zip
 Command sem in package parallel                         Command gp in package pari
 Command fpp in package pathpicker
 Command pb in package pb                                Command pet in package pet
 Command php in package php
 Command pil in package picolisp
 Command ode in package plotutils from the x11-repo repository
 Command ps in package procps
 Command cct in package proj
 Command pd in package proot-distro
 Command pup in package pup                              Command pv in package pv                                Command pip in package python-pip
 Command q in package q-dns-client                       Command moc in package qt5-qtbase from the x11-repo repository                                                  Command qml in package qt5-qtdeclarative from the x11-repo repository                                           Command qev in package qt5-qttools from the x11-repo repository
 Command qjs in package quickjs
 Command r2 in package radare2
 Command rbw in package rbw                              Command rc in package rc
 Command ci in package rcs
 Command rem in package remind
 Command icp in package renameutils
 Command rig in package rig
 Command rip in package rip2
 Command rg in package ripgrep
 Command rga in package ripgrep-all
 Command rnr in package rnr
 Command rpm in package rpm
 Command rq in package rq                                Command erb in package ruby
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command net in package samba
 Command scc in package scc                              Command sd in package sd
 Command srm in package secure-delete                    Command sed in package sed
 Command shc in package shc
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command fls in package sleuthkit
 Command gst in package smalltalk
 Command rec in package sox
 Command st in package st from the x11-repo repository   Command svn in package subversion
 Command sun in package sun                              Command sr in package surfraw
 Command tar in package tar
 Command tsp in package task-spooler
 Command tcc in package tcc
 Command nns in package tcllib
 Command tdl in package tdl                              Command tea in package tea
 Command tsh in package teleport-tsh
 Command am in package termux-am                         Command cmd in package termux-tools
 Command ebb in package texlive-bin
 Command tig in package tig
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command tor in package tor
 Command trz in package trzsz-go                         Command tsu in package tsu
 Command tut in package tut
 Command tjs in package txikijs                          Command ug in package ugrep
 Command up in package up
 Command upx in package upx
 Command cal in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository                                                      Command vt in package virustotal-cli
 Command vi in package vis                               Command viu in package viu
 Command vlc in package vlc
 Command vlc in package vlc-qt from the x11-repo repository
 Command vtm in package vtm
 Command w3m in package w3m
 Command wg in package wireguard-tools
 Command wiz in package wiz
 Command wol in package wol
 Command wrk in package wrk
 Command x2x in package x2x from the x11-repo repository
 Command xh in package xh
 Command xml in package xmlstarlet
 Command X in package xorg-server from the x11-repo repository                                                   Command twm in package xorg-twm from the x11-repo repository
 Command xev in package xorg-xev from the x11-repo repository
 Command xxd in package xxd                              Command xz in package xz-utils
 Command yad in package yad from the x11-repo repository
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zip in package zip                              Command zk in package zk
 Command znc in package znc
 Command zsh in package zsh
No command │ found, did you mean:
 Command 7zz in package 7zip
 Command ack in package ack-grep
 Command acr in package acr
 Command age in package age
 Command agg in package agg
 Command aha in package aha
 Command adb in package android-tools
 Command ant in package ant
 Command ab in package apache2                           Command apt in package apt
 Command arj in package arj
 Command ark in package ark from the x11-repo repository
 Command a2x in package asciidoc
 Command asy in package asymptote                        Command at in package at
 Command als in package atool                            Command aws in package awscli
 Command bat in package bat                              Command bc in package bc
 Command bsh in package beanshell
 Command bed in package bed
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command atc in package bsd-games
 Command buf in package buf
 Command ash in package busybox                          Command bvi in package bvi
 Command cfm in package cfm
 Command cjs in package cjs from the x11-repo repository
 Command c++ in package clang
 Command ccr in package codecrypt
 Command cbc in package coinor-cbc
 Command clp in package coinor-clp
 Command ctr in package containerd from the root-repo repository                                                 Command [ in package coreutils
 Command ocs in package cscope                           Command lp in package cups
 Command cvs in package cvs                              Command d8 in package d8
 Command dar in package dar
 Command sh in package dash
 Command dlv in package delve
 Command dia in package dia from the x11-repo repository
 Command cmp in package diffutils
 Command bzz in package djvulibre
 Command dig in package dnsutils
 Command scp in package dropbear
 Command dtc in package dtc
 Command dte in package dte
 Command dua in package dua
 Command duc in package duc
 Command duf in package duf                              Command duk in package duktape
 Command dwm in package dwm from the x11-repo repository Command dx in package dx
 Command e16 in package e16 from the x11-repo repository
 Command ecj in package ecj                              Command ecl in package ecl
 Command ed in package ed                                Command eja in package eja
 Command ef in package electric-fence
 Command iex in package elixir
 Command eog in package eog from the x11-repo repository
 Command eom in package eom from the x11-repo repository
 Command erl in package erlang
 Command et in package et
 Command tsh in package etsh
 Command eww in package eww from the x11-repo repository
 Command eza in package eza                              Command fcp in package fcp
 Command fd in package fd                                Command fdm in package fdm                              Command feh in package feh from the x11-repo repository
 Command fff in package fff                              Command fio in package fio from the root-repo repository                                                        Command bbc in package flang                            Command fm in package fm
 Command fx in package fx
 Command fzf in package fzf                              Command fzy in package fzy
 Command gac in package gap
 Command dl in package gatling                           Command awk in package gawk
 Command gbt in package gbt
 Command gdb in package gdb                              Command gdl in package gdrive-downloader
 Command gdu in package gdu
 Command era in package geth-utils                       Command gh in package gh
 Command ghc in package ghc
 Command gs in package ghostscript
 Command git in package git
 Command ein in package gitoxide
 Command gio in package glib                             Command gn in package gn
 Command gpg in package gnupg
 Command go in package golang
 Command tsc in package gotify
 Command gm in package graphicsmagick
 Command dot in package graphviz
 Command eqn in package groff
 Command gsf in package gsf-tools
 Command gum in package gum
 Command gw in package gw from the x11-repo repository
 Command ghb in package handbrake from the x11-repo repository
 Command hx in package helix
 Command hcd in package hfsutils
 Command hh in package hstr
 Command hub in package hub
 Command hut in package hut
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command iat in package iat
 Command ftp in package inetutils
 Command ip in package iproute2
 Command na6 in package ipv6toolkit
 Command vvp in package iverilog
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command joe in package joe
 Command jq in package jq
 Command jql in package jql
 Command joe in package jupp
 Command jwm in package jwm from the x11-repo repository
 Command k9s in package k9s
 Command kak in package kakoune
 Command k in package kona
 Command ksu in package krb5
 Command dub in package ldc
 Command ldd in package ldd
 Command lf in package lf
 Command lha in package lhasa
 Command pl in package libgnustep-base
 Command psl in package libpsl
 Command h3 in package libuber-h3
 Command cvt in package libxcvt from the x11-repo repository
 Command lit in package lit
 Command lld in package lld
 Command llc in package llvm
 Command not in package llvm-tools
 Command lnd in package lnd
 Command ksh in package loksh
 Command lr in package lr
 Command lrb in package lrzsz
 Command lsd in package lsd                              Command lua in package lua51
 Command lua in package lua52
 Command lua in package lua53
 Command lua in package lua54
 Command lua in package lua55
 Command lux in package lux
 Command lx in package lux-cli
 Command lvm in package lvm2 from the root-repo repository
 Command lyx in package lyx from the x11-repo repository
 Command lz4 in package lz4
 Command m4 in package m4
 Command ali in package mailutils                        Command man in package mandoc
 Command mvn in package maven
 Command mc in package mc
 Command mdp in package mdp
 Command mdb in package mercury
 Command ray in package mesa-demos from the x11-repo repository
 Command mg in package mg
 Command mlr in package miller
 Command al in package mono
 Command mop in package mop
 Command pee in package moreutils
 Command mpc in package mpc
 Command mpd in package mpd
 Command mpv in package mpv
 Command mpv in package mpv-x from the x11-repo repository
 Command lz in package mtools
 Command mtr in package mtr from the root-repo repository
 Command mu in package mu
 Command mr in package myrepos
 Command psc in package n-t-roff-sc
 Command tic in package ncurses-utils
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command arp in package net-tools
 Command nc in package netcat-openbsd
 Command nim in package nim
 Command nc in package nmap
 Command ali in package nmh
 Command nnn in package nnn
 Command nms in package no-more-secrets
 Command npm in package npm
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command oma in package oma
 Command iv in package openimageio from the x11-repo repository
 Command jar in package openjdk-21
 Command jar in package openjdk-25
 Command scp in package openssh
 Command o in package orbiton
 Command 7z in package p7zip
 Command sem in package parallel
 Command gp in package pari
 Command fpp in package pathpicker
 Command pb in package pb
 Command pet in package pet
 Command php in package php
 Command pil in package picolisp
 Command ode in package plotutils from the x11-repo repository
 Command ps in package procps
 Command cct in package proj
 Command pd in package proot-distro
 Command pup in package pup
 Command pv in package pv
 Command pip in package python-pip
 Command q in package q-dns-client
 Command moc in package qt5-qtbase from the x11-repo repository
 Command qml in package qt5-qtdeclarative from the x11-repo repository
 Command qev in package qt5-qttools from the x11-repo repository
 Command qjs in package quickjs
 Command r2 in package radare2
 Command rbw in package rbw
 Command rc in package rc
 Command ci in package rcs
 Command rem in package remind
 Command icp in package renameutils
 Command rig in package rig                              Command rip in package rip2
 Command rg in package ripgrep
 Command rga in package ripgrep-all                      Command rnr in package rnr
 Command rpm in package rpm
 Command rq in package rq
 Command erb in package ruby
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command net in package samba
 Command scc in package scc
 Command sd in package sd
 Command srm in package secure-delete
 Command sed in package sed
 Command shc in package shc
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command fls in package sleuthkit
 Command gst in package smalltalk
 Command rec in package sox
 Command st in package st from the x11-repo repository
 Command svn in package subversion
 Command sun in package sun
 Command sr in package surfraw
 Command tar in package tar
 Command tsp in package task-spooler
 Command tcc in package tcc
 Command nns in package tcllib
 Command tdl in package tdl
 Command tea in package tea
 Command tsh in package teleport-tsh
 Command am in package termux-am
 Command cmd in package termux-tools
 Command ebb in package texlive-bin
 Command tig in package tig
 Command sn in package tin-summer
 Command tf in package tinyfugue                         Command tor in package tor
 Command trz in package trzsz-go
 Command tsu in package tsu
 Command tut in package tut
 Command tjs in package txikijs
 Command ug in package ugrep                             Command up in package up
 Command upx in package upx
 Command cal in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command viu in package viu
 Command vlc in package vlc
 Command vlc in package vlc-qt from the x11-repo repository
 Command vtm in package vtm
 Command w3m in package w3m
 Command wg in package wireguard-tools
 Command wiz in package wiz                              Command wol in package wol
 Command wrk in package wrk
 Command x2x in package x2x from the x11-repo repository
 Command xh in package xh
 Command xml in package xmlstarlet
 Command X in package xorg-server from the x11-repo repository                                                   Command twm in package xorg-twm from the x11-repo repository
 Command xev in package xorg-xev from the x11-repo repository
 Command xxd in package xxd
 Command xz in package xz-utils
 Command yad in package yad from the x11-repo repository
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zip in package zip
 Command zk in package zk
 Command znc in package znc
 Command zsh in package zsh
No command │ found, did you mean:
 Command 7zz in package 7zip
 Command ack in package ack-grep
 Command acr in package acr
 Command age in package age
 Command agg in package agg
 Command aha in package aha
 Command adb in package android-tools
 Command ant in package ant
 Command ab in package apache2
 Command apt in package apt
 Command arj in package arj
 Command ark in package ark from the x11-repo repository
 Command a2x in package asciidoc
 Command asy in package asymptote
 Command at in package at
 Command als in package atool
 Command aws in package awscli
 Command bat in package bat
 Command bc in package bc
 Command bsh in package beanshell
 Command bed in package bed
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command atc in package bsd-games
 Command buf in package buf
 Command ash in package busybox
 Command bvi in package bvi
 Command cfm in package cfm
 Command cjs in package cjs from the x11-repo repository
 Command c++ in package clang
 Command ccr in package codecrypt
 Command cbc in package coinor-cbc
 Command clp in package coinor-clp
 Command ctr in package containerd from the root-repo repository
 Command [ in package coreutils
 Command ocs in package cscope
 Command lp in package cups
 Command cvs in package cvs
 Command d8 in package d8
 Command dar in package dar
 Command sh in package dash
 Command dlv in package delve
 Command dia in package dia from the x11-repo repository
 Command cmp in package diffutils
 Command bzz in package djvulibre
 Command dig in package dnsutils
 Command scp in package dropbear
 Command dtc in package dtc
 Command dte in package dte                              Command dua in package dua
 Command duc in package duc
 Command duf in package duf                              Command duk in package duktape
 Command dwm in package dwm from the x11-repo repository
 Command dx in package dx
 Command e16 in package e16 from the x11-repo repository
 Command ecj in package ecj
 Command ecl in package ecl
 Command ed in package ed
 Command eja in package eja
 Command ef in package electric-fence
 Command iex in package elixir
 Command eog in package eog from the x11-repo repository
 Command eom in package eom from the x11-repo repository
 Command erl in package erlang
 Command et in package et
 Command tsh in package etsh
 Command eww in package eww from the x11-repo repository
 Command eza in package eza
 Command fcp in package fcp
 Command fd in package fd
 Command fdm in package fdm
 Command feh in package feh from the x11-repo repository
 Command fff in package fff
 Command fio in package fio from the root-repo repository
 Command bbc in package flang
 Command fm in package fm
 Command fx in package fx
 Command fzf in package fzf
 Command fzy in package fzy
 Command gac in package gap
 Command dl in package gatling
 Command awk in package gawk
 Command gbt in package gbt
 Command gdb in package gdb
 Command gdl in package gdrive-downloader                Command gdu in package gdu
 Command era in package geth-utils
 Command gh in package gh
 Command ghc in package ghc
 Command gs in package ghostscript
 Command git in package git                              Command ein in package gitoxide
 Command gio in package glib
 Command gn in package gn
 Command gpg in package gnupg
 Command go in package golang
 Command tsc in package gotify
 Command gm in package graphicsmagick
 Command dot in package graphviz
 Command eqn in package groff
 Command gsf in package gsf-tools
 Command gum in package gum
 Command gw in package gw from the x11-repo repository
 Command ghb in package handbrake from the x11-repo repository
 Command hx in package helix
 Command hcd in package hfsutils
 Command hh in package hstr
 Command hub in package hub
 Command hut in package hut
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command iat in package iat
 Command ftp in package inetutils
 Command ip in package iproute2
 Command na6 in package ipv6toolkit
 Command vvp in package iverilog
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command joe in package joe
 Command jq in package jq
 Command jql in package jql
 Command joe in package jupp
 Command jwm in package jwm from the x11-repo repository
 Command k9s in package k9s
 Command kak in package kakoune
 Command k in package kona
 Command ksu in package krb5
 Command dub in package ldc
 Command ldd in package ldd
 Command lf in package lf
 Command lha in package lhasa
 Command pl in package libgnustep-base
 Command psl in package libpsl
 Command h3 in package libuber-h3
 Command cvt in package libxcvt from the x11-repo repository
 Command lit in package lit
 Command lld in package lld
 Command llc in package llvm
 Command not in package llvm-tools
 Command lnd in package lnd
 Command ksh in package loksh
 Command lr in package lr
 Command lrb in package lrzsz
 Command lsd in package lsd
 Command lua in package lua51
 Command lua in package lua52
 Command lua in package lua53
 Command lua in package lua54
 Command lua in package lua55
 Command lux in package lux
 Command lx in package lux-cli
 Command lvm in package lvm2 from the root-repo repository
 Command lyx in package lyx from the x11-repo repository
 Command lz4 in package lz4
 Command m4 in package m4
 Command ali in package mailutils
 Command man in package mandoc
 Command mvn in package maven
 Command mc in package mc
 Command mdp in package mdp
 Command mdb in package mercury
 Command ray in package mesa-demos from the x11-repo repository
 Command mg in package mg
 Command mlr in package miller
 Command al in package mono
 Command mop in package mop
 Command pee in package moreutils
 Command mpc in package mpc
 Command mpd in package mpd
 Command mpv in package mpv
 Command mpv in package mpv-x from the x11-repo repository
 Command lz in package mtools
 Command mtr in package mtr from the root-repo repository                                                        Command mu in package mu
 Command mr in package myrepos
 Command psc in package n-t-roff-sc                      Command tic in package ncurses-utils
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command arp in package net-tools
 Command nc in package netcat-openbsd
 Command nim in package nim
 Command nc in package nmap
 Command ali in package nmh
 Command nnn in package nnn
 Command nms in package no-more-secrets
 Command npm in package npm
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command oma in package oma
 Command iv in package openimageio from the x11-repo repository
 Command jar in package openjdk-21
 Command jar in package openjdk-25
 Command scp in package openssh
 Command o in package orbiton
 Command 7z in package p7zip
 Command sem in package parallel
 Command gp in package pari
 Command fpp in package pathpicker
 Command pb in package pb
 Command pet in package pet
 Command php in package php
 Command pil in package picolisp
 Command ode in package plotutils from the x11-repo repository
 Command ps in package procps
 Command cct in package proj                             Command pd in package proot-distro
 Command pup in package pup
 Command pv in package pv
 Command pip in package python-pip
 Command q in package q-dns-client
 Command moc in package qt5-qtbase from the x11-repo repository
 Command qml in package qt5-qtdeclarative from the x11-repo repository
 Command qev in package qt5-qttools from the x11-repo repository
 Command qjs in package quickjs
 Command r2 in package radare2
 Command rbw in package rbw
 Command rc in package rc
 Command ci in package rcs                               Command rem in package remind
 Command icp in package renameutils
 Command rig in package rig
 Command rip in package rip2
 Command rg in package ripgrep
 Command rga in package ripgrep-all
 Command rnr in package rnr
 Command rpm in package rpm
 Command rq in package rq
 Command erb in package ruby
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command net in package samba
 Command scc in package scc
 Command sd in package sd
 Command srm in package secure-delete
 Command sed in package sed
 Command shc in package shc
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command fls in package sleuthkit
 Command gst in package smalltalk
 Command rec in package sox
 Command st in package st from the x11-repo repository
 Command svn in package subversion
 Command sun in package sun
 Command sr in package surfraw
 Command tar in package tar
 Command tsp in package task-spooler
 Command tcc in package tcc
 Command nns in package tcllib
 Command tdl in package tdl
 Command tea in package tea
 Command tsh in package teleport-tsh
 Command am in package termux-am
 Command cmd in package termux-tools
 Command ebb in package texlive-bin
 Command tig in package tig
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command tor in package tor
 Command trz in package trzsz-go
 Command tsu in package tsu
 Command tut in package tut
 Command tjs in package txikijs
 Command ug in package ugrep
 Command up in package up
 Command upx in package upx
 Command cal in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command viu in package viu
 Command vlc in package vlc
 Command vlc in package vlc-qt from the x11-repo repository
 Command vtm in package vtm
 Command w3m in package w3m
 Command wg in package wireguard-tools
 Command wiz in package wiz
 Command wol in package wol
 Command wrk in package wrk
 Command x2x in package x2x from the x11-repo repository
 Command xh in package xh
 Command xml in package xmlstarlet
 Command X in package xorg-server from the x11-repo repository
 Command twm in package xorg-twm from the x11-repo repository                                                    Command xev in package xorg-xev from the x11-repo repository
 Command xxd in package xxd
 Command xz in package xz-utils
 Command yad in package yad from the x11-repo repository
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zip in package zip
 Command zk in package zk
 Command znc in package znc
 Command zsh in package zsh
No command │ found, did you mean:
 Command 7zz in package 7zip
 Command ack in package ack-grep
 Command acr in package acr
 Command age in package age
 Command agg in package agg
 Command aha in package aha
 Command adb in package android-tools
 Command ant in package ant
 Command ab in package apache2
 Command apt in package apt
 Command arj in package arj                              Command ark in package ark from the x11-repo repository
 Command a2x in package asciidoc                         Command asy in package asymptote
 Command at in package at
 Command als in package atool
 Command aws in package awscli                           Command bat in package bat
 Command bc in package bc
 Command bsh in package beanshell
 Command bed in package bed
 Command ar in package binutils                          Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command atc in package bsd-games
 Command buf in package buf
 Command ash in package busybox                          Command bvi in package bvi
 Command cfm in package cfm                              Command cjs in package cjs from the x11-repo repository
 Command c++ in package clang                            Command ccr in package codecrypt
 Command cbc in package coinor-cbc
 Command clp in package coinor-clp                       Command ctr in package containerd from the root-repo repository
 Command [ in package coreutils
 Command ocs in package cscope
 Command lp in package cups
 Command cvs in package cvs
 Command d8 in package d8                                Command dar in package dar
 Command sh in package dash
 Command dlv in package delve
 Command dia in package dia from the x11-repo repository
 Command cmp in package diffutils
 Command bzz in package djvulibre                        Command dig in package dnsutils
 Command scp in package dropbear                         Command dtc in package dtc
 Command dte in package dte
 Command dua in package dua
 Command duc in package duc                              Command duf in package duf
 Command duk in package duktape
 Command dwm in package dwm from the x11-repo repository
 Command dx in package dx
 Command e16 in package e16 from the x11-repo repository
 Command ecj in package ecj
 Command ecl in package ecl
 Command ed in package ed
 Command eja in package eja
 Command ef in package electric-fence
 Command iex in package elixir
 Command eog in package eog from the x11-repo repository
 Command eom in package eom from the x11-repo repository
 Command erl in package erlang
 Command et in package et
 Command tsh in package etsh
 Command eww in package eww from the x11-repo repository
 Command eza in package eza
 Command fcp in package fcp
 Command fd in package fd
 Command fdm in package fdm
 Command feh in package feh from the x11-repo repository
 Command fff in package fff                              Command fio in package fio from the root-repo repository                                                        Command bbc in package flang
 Command fm in package fm
 Command fx in package fx
 Command fzf in package fzf
 Command fzy in package fzy                              Command gac in package gap
 Command dl in package gatling
 Command awk in package gawk
 Command gbt in package gbt
 Command gdb in package gdb
 Command gdl in package gdrive-downloader
 Command gdu in package gdu
 Command era in package geth-utils
 Command gh in package gh
 Command ghc in package ghc
 Command gs in package ghostscript                       Command git in package git
 Command ein in package gitoxide                         Command gio in package glib
 Command gn in package gn                                Command gpg in package gnupg
 Command go in package golang                            Command tsc in package gotify
 Command gm in package graphicsmagick
 Command dot in package graphviz
 Command eqn in package groff
 Command gsf in package gsf-tools
 Command gum in package gum                              Command gw in package gw from the x11-repo repository
 Command ghb in package handbrake from the x11-repo repository
 Command hx in package helix                             Command hcd in package hfsutils
 Command hh in package hstr
 Command hub in package hub                              Command hut in package hut
 Command hz in package hz                                Command i3 in package i3 from the x11-repo repository
 Command iat in package iat
 Command ftp in package inetutils                        Command ip in package iproute2
 Command na6 in package ipv6toolkit                      Command vvp in package iverilog
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command joe in package joe
 Command jq in package jq
 Command jql in package jql
 Command joe in package jupp
 Command jwm in package jwm from the x11-repo repository
 Command k9s in package k9s                              Command kak in package kakoune
 Command k in package kona                               Command ksu in package krb5
 Command dub in package ldc
 Command ldd in package ldd
 Command lf in package lf
 Command lha in package lhasa
 Command pl in package libgnustep-base
 Command psl in package libpsl                           Command h3 in package libuber-h3
 Command cvt in package libxcvt from the x11-repo repository                                                     Command lit in package lit
 Command lld in package lld
 Command llc in package llvm
 Command not in package llvm-tools
 Command lnd in package lnd                              Command ksh in package loksh
 Command lr in package lr
 Command lrb in package lrzsz                            Command lsd in package lsd
 Command lua in package lua51
 Command lua in package lua52
 Command lua in package lua53
 Command lua in package lua54
 Command lua in package lua55
 Command lux in package lux
 Command lx in package lux-cli
 Command lvm in package lvm2 from the root-repo repository
 Command lyx in package lyx from the x11-repo repository
 Command lz4 in package lz4
 Command m4 in package m4
 Command ali in package mailutils
 Command man in package mandoc
 Command mvn in package maven
 Command mc in package mc                                Command mdp in package mdp
 Command mdb in package mercury                          Command ray in package mesa-demos from the x11-repo repository
 Command mg in package mg
 Command mlr in package miller
 Command al in package mono
 Command mop in package mop
 Command pee in package moreutils
 Command mpc in package mpc
 Command mpd in package mpd
 Command mpv in package mpv
 Command mpv in package mpv-x from the x11-repo repository                                                       Command lz in package mtools
 Command mtr in package mtr from the root-repo repository
 Command mu in package mu                                Command mr in package myrepos
 Command psc in package n-t-roff-sc                      Command tic in package ncurses-utils
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command arp in package net-tools
 Command nc in package netcat-openbsd
 Command nim in package nim
 Command nc in package nmap
 Command ali in package nmh
 Command nnn in package nnn
 Command nms in package no-more-secrets                  Command npm in package npm
 Command pp in package nss-utils
 Command nu in package nushell                           Command nx in package nxengine from the x11-repo repository
 Command ol in package ol                                Command oma in package oma
 Command iv in package openimageio from the x11-repo repository
 Command jar in package openjdk-21
 Command jar in package openjdk-25                       Command scp in package openssh
 Command o in package orbiton                            Command 7z in package p7zip                             Command sem in package parallel
 Command gp in package pari                              Command fpp in package pathpicker
 Command pb in package pb                                Command pet in package pet
 Command php in package php
 Command pil in package picolisp                         Command ode in package plotutils from the x11-repo repository                                                   Command ps in package procps
 Command cct in package proj
 Command pd in package proot-distro                      Command pup in package pup
 Command pv in package pv                                Command pip in package python-pip
 Command q in package q-dns-client                       Command moc in package qt5-qtbase from the x11-repo repository
 Command qml in package qt5-qtdeclarative from the x11-repo repository
 Command qev in package qt5-qttools from the x11-repo repository
 Command qjs in package quickjs
 Command r2 in package radare2                           Command rbw in package rbw
 Command rc in package rc                                Command ci in package rcs
 Command rem in package remind                           Command icp in package renameutils                      Command rig in package rig
 Command rip in package rip2                             Command rg in package ripgrep
 Command rga in package ripgrep-all                      Command rnr in package rnr
 Command rpm in package rpm
 Command rq in package rq                                Command erb in package ruby
 Command ri in package ruby-ri
 Command sv in package runit                             Command rw in package rw
 Command net in package samba
 Command scc in package scc                              Command sd in package sd
 Command srm in package secure-delete
 Command sed in package sed                              Command shc in package shc
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command fls in package sleuthkit
 Command gst in package smalltalk
 Command rec in package sox                              Command st in package st from the x11-repo repository
 Command svn in package subversion
 Command sun in package sun
 Command sr in package surfraw
 Command tar in package tar
 Command tsp in package task-spooler
 Command tcc in package tcc
 Command nns in package tcllib
 Command tdl in package tdl
 Command tea in package tea
 Command tsh in package teleport-tsh
 Command am in package termux-am
 Command cmd in package termux-tools
 Command ebb in package texlive-bin                      Command tig in package tig
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command tor in package tor
 Command trz in package trzsz-go
 Command tsu in package tsu
 Command tut in package tut
 Command tjs in package txikijs
 Command ug in package ugrep
 Command up in package up
 Command upx in package upx
 Command cal in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command viu in package viu
 Command vlc in package vlc
 Command vlc in package vlc-qt from the x11-repo repository
 Command vtm in package vtm
 Command w3m in package w3m
 Command wg in package wireguard-tools
 Command wiz in package wiz
 Command wol in package wol
 Command wrk in package wrk
 Command x2x in package x2x from the x11-repo repository
 Command xh in package xh
 Command xml in package xmlstarlet
 Command X in package xorg-server from the x11-repo repository
 Command twm in package xorg-twm from the x11-repo repository
 Command xev in package xorg-xev from the x11-repo repository
 Command xxd in package xxd
 Command xz in package xz-utils
 Command yad in package yad from the x11-repo repository
 Command ya in package yazi                              Command yq in package yq
 Command z3 in package z3
 Command zip in package zip
 Command zk in package zk
 Command znc in package znc
 Command zsh in package zsh
No command │ found, did you mean:
 Command 7zz in package 7zip
 Command ack in package ack-grep
 Command acr in package acr
 Command age in package age
 Command agg in package agg
 Command aha in package aha
 Command adb in package android-tools
 Command ant in package ant
 Command ab in package apache2
 Command apt in package apt
 Command arj in package arj
 Command ark in package ark from the x11-repo repository
 Command a2x in package asciidoc
 Command asy in package asymptote
 Command at in package at
 Command als in package atool
 Command aws in package awscli
 Command bat in package bat
 Command bc in package bc
 Command bsh in package beanshell
 Command bed in package bed
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command atc in package bsd-games
 Command buf in package buf
 Command ash in package busybox
 Command bvi in package bvi
 Command cfm in package cfm
 Command cjs in package cjs from the x11-repo repository
 Command c++ in package clang
 Command ccr in package codecrypt
 Command cbc in package coinor-cbc
 Command clp in package coinor-clp                       Command ctr in package containerd from the root-repo repository
 Command [ in package coreutils
 Command ocs in package cscope
 Command lp in package cups
 Command cvs in package cvs
 Command d8 in package d8
 Command dar in package dar
 Command sh in package dash
 Command dlv in package delve
 Command dia in package dia from the x11-repo repository
 Command cmp in package diffutils
 Command bzz in package djvulibre
 Command dig in package dnsutils
 Command scp in package dropbear
 Command dtc in package dtc
 Command dte in package dte
 Command dua in package dua
 Command duc in package duc
 Command duf in package duf
 Command duk in package duktape
 Command dwm in package dwm from the x11-repo repository
 Command dx in package dx
 Command e16 in package e16 from the x11-repo repository
 Command ecj in package ecj
 Command ecl in package ecl
 Command ed in package ed
 Command eja in package eja
 Command ef in package electric-fence
 Command iex in package elixir
 Command eog in package eog from the x11-repo repository Command eom in package eom from the x11-repo repository
 Command erl in package erlang
 Command et in package et
 Command tsh in package etsh
 Command eww in package eww from the x11-repo repository
 Command eza in package eza
 Command fcp in package fcp
 Command fd in package fd
 Command fdm in package fdm
 Command feh in package feh from the x11-repo repository
 Command fff in package fff
 Command fio in package fio from the root-repo repository
 Command bbc in package flang
 Command fm in package fm
 Command fx in package fx
 Command fzf in package fzf
 Command fzy in package fzy
 Command gac in package gap
 Command dl in package gatling
 Command awk in package gawk
 Command gbt in package gbt
 Command gdb in package gdb
 Command gdl in package gdrive-downloader
 Command gdu in package gdu
 Command era in package geth-utils
 Command gh in package gh
 Command ghc in package ghc
 Command gs in package ghostscript
 Command git in package git
 Command ein in package gitoxide
 Command gio in package glib                             Command gn in package gn
 Command gpg in package gnupg
 Command go in package golang
 Command tsc in package gotify
 Command gm in package graphicsmagick
 Command dot in package graphviz
 Command eqn in package groff
 Command gsf in package gsf-tools
 Command gum in package gum
 Command gw in package gw from the x11-repo repository
 Command ghb in package handbrake from the x11-repo repository
 Command hx in package helix
 Command hcd in package hfsutils
 Command hh in package hstr
 Command hub in package hub
 Command hut in package hut
 Command hz in package hz                                Command i3 in package i3 from the x11-repo repository
 Command iat in package iat
 Command ftp in package inetutils
 Command ip in package iproute2
 Command na6 in package ipv6toolkit
 Command vvp in package iverilog
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command joe in package joe
 Command jq in package jq
 Command jql in package jql                              Command joe in package jupp
 Command jwm in package jwm from the x11-repo repository
 Command k9s in package k9s
 Command kak in package kakoune
 Command k in package kona
 Command ksu in package krb5
 Command dub in package ldc
 Command ldd in package ldd
 Command lf in package lf
 Command lha in package lhasa                            Command pl in package libgnustep-base
 Command psl in package libpsl
 Command h3 in package libuber-h3                        Command cvt in package libxcvt from the x11-repo repository
 Command lit in package lit
 Command lld in package lld
 Command llc in package llvm
 Command not in package llvm-tools
 Command lnd in package lnd
 Command ksh in package loksh
 Command lr in package lr
 Command lrb in package lrzsz
 Command lsd in package lsd
 Command lua in package lua51
 Command lua in package lua52
 Command lua in package lua53
 Command lua in package lua54
 Command lua in package lua55
 Command lux in package lux
 Command lx in package lux-cli                           Command lvm in package lvm2 from the root-repo repository
 Command lyx in package lyx from the x11-repo repository
 Command lz4 in package lz4                              Command m4 in package m4
 Command ali in package mailutils
 Command man in package mandoc
 Command mvn in package maven
 Command mc in package mc
 Command mdp in package mdp
 Command mdb in package mercury
 Command ray in package mesa-demos from the x11-repo repository
 Command mg in package mg
 Command mlr in package miller
 Command al in package mono
 Command mop in package mop
 Command pee in package moreutils                        Command mpc in package mpc
 Command mpd in package mpd
 Command mpv in package mpv
 Command mpv in package mpv-x from the x11-repo repository
 Command lz in package mtools
 Command mtr in package mtr from the root-repo repository
 Command mu in package mu                                Command mr in package myrepos
 Command psc in package n-t-roff-sc                      Command tic in package ncurses-utils
 Command ne in package ne                                Command ex in package neovim-nightly,neovim
 Command arp in package net-tools
 Command nc in package netcat-openbsd
 Command nim in package nim
 Command nc in package nmap
 Command ali in package nmh
 Command nnn in package nnn
 Command nms in package no-more-secrets
 Command npm in package npm
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository
 Command ol in package ol
 Command oma in package oma
 Command iv in package openimageio from the x11-repo repository
 Command jar in package openjdk-21
 Command jar in package openjdk-25
 Command scp in package openssh
 Command o in package orbiton
 Command 7z in package p7zip
 Command sem in package parallel
 Command gp in package pari
 Command fpp in package pathpicker
 Command pb in package pb
 Command pet in package pet
 Command php in package php
 Command pil in package picolisp
 Command ode in package plotutils from the x11-repo repository
 Command ps in package procps
 Command cct in package proj
 Command pd in package proot-distro
 Command pup in package pup
 Command pv in package pv
 Command pip in package python-pip
 Command q in package q-dns-client
 Command moc in package qt5-qtbase from the x11-repo repository
 Command qml in package qt5-qtdeclarative from the x11-repo repository
 Command qev in package qt5-qttools from the x11-repo repository
 Command qjs in package quickjs
 Command r2 in package radare2
 Command rbw in package rbw
 Command rc in package rc
 Command ci in package rcs
 Command rem in package remind
 Command icp in package renameutils
 Command rig in package rig
 Command rip in package rip2
 Command rg in package ripgrep
 Command rga in package ripgrep-all
 Command rnr in package rnr
 Command rpm in package rpm
 Command rq in package rq
 Command erb in package ruby
 Command ri in package ruby-ri                           Command sv in package runit
 Command rw in package rw
 Command net in package samba
 Command scc in package scc
 Command sd in package sd
 Command srm in package secure-delete                    Command sed in package sed
 Command shc in package shc
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command fls in package sleuthkit
 Command gst in package smalltalk
 Command rec in package sox
 Command st in package st from the x11-repo repository
 Command svn in package subversion
 Command sun in package sun
 Command sr in package surfraw                           Command tar in package tar
 Command tsp in package task-spooler                     Command tcc in package tcc
 Command nns in package tcllib                           Command tdl in package tdl
 Command tea in package tea
 Command tsh in package teleport-tsh
 Command am in package termux-am
 Command cmd in package termux-tools
 Command ebb in package texlive-bin
 Command tig in package tig
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command tor in package tor
 Command trz in package trzsz-go
 Command tsu in package tsu
 Command tut in package tut
 Command tjs in package txikijs
 Command ug in package ugrep
 Command up in package up
 Command upx in package upx
 Command cal in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command viu in package viu
 Command vlc in package vlc
 Command vlc in package vlc-qt from the x11-repo repository
 Command vtm in package vtm
 Command w3m in package w3m
 Command wg in package wireguard-tools
 Command wiz in package wiz
 Command wol in package wol
 Command wrk in package wrk
 Command x2x in package x2x from the x11-repo repository
 Command xh in package xh
 Command xml in package xmlstarlet
 Command X in package xorg-server from the x11-repo repository
 Command twm in package xorg-twm from the x11-repo repository
 Command xev in package xorg-xev from the x11-repo repository                                                    Command xxd in package xxd
 Command xz in package xz-utils
 Command yad in package yad from the x11-repo repository
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zip in package zip
 Command zk in package zk
 Command znc in package znc
 Command zsh in package zsh
├──: command not found
└──: command not found
~ $ import { createClient } from '@supabase/supabase-js';
export const supabase = createClient('SUA_URL', 'SUA_CHAVE');
The program import is not installed. Install it by executing:
 pkg install imagemagick
bash: syntax error near unexpected token `('
~ $ import React from 'react';
import { createStackNavigator } from '@react-navigation/stack';
import LoginScreen from '../screens/LoginScreen';
import HomeScreen from '../screens/HomeScreen';

const Stack = createStackNavigator();

export default function AppNavigator() {
  return (
    <Stack.Navigator screenOptions={{ headerShown: false }}>
      <Stack.Screen name="Login" component={LoginScreen} />
      <Stack.Screen name="Home" component={HomeScreen} />                                                           </Stack.Navigator>
  );
}
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
bash: syntax error near unexpected token `('            bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'
~ $ import React, { useState, useEffect } from 'react'; import { NavigationContainer } from '@react-navigation/native';                                                 import { createStackNavigator } from '@react-navigation/stack';                                                 import {
  View, Text, TextInput, TouchableOpacity, StyleSheet,
  SafeAreaView, ScrollView, StatusBar, Alert, Dimensions, Image
} from 'react-native';
import { LineChart } from 'react-native-chart-kit';
import * as ImagePicker from 'expo-image-picker';

const Stack = createStackNavigator();
const screenWidth = Dimensions.get("window").width;     
// --- TELA DE LOGIN ---
function LoginScreen({ navigation }) {                    const [email, setEmail] = useState('');
  const [pass, setPass] = useState('');
                                                          const handleLogin = () => {
    if (email === 'admin@pro.com' && pass === '123456') {
      navigation.replace('Home');                           } else {
      Alert.alert('Erro', 'Credenciais inválidas');
    }
  };

  return (
    <View style={styles.loginContainer}>
      <Text style={styles.loginLogo}>Contabilidade<Text style={{color: '#1d4ed8'}}>PRO</Text></Text>
      <TextInput style={styles.input} placeholder="E-mail" onChangeText={setEmail} autoCapitalize="none" />
      <TextInput style={styles.input} placeholder="Senha" secureTextEntry onChangeText={setPass} />
      <TouchableOpacity style={styles.mainButton} onPress={handleLogin}>
        <Text style={styles.buttonText}>Entrar no Sistema</Text>
      </TouchableOpacity>
    </View>
  );
}
                                                        // --- DASHBOARD PRINCIPAL ---
function HomeScreen({ navigation }) {
  return (
    <SafeAreaView style={styles.container}>
      <StatusBar barStyle="light-content" backgroundColor="#1d4ed8" />
      <ScrollView showsVerticalScrollIndicator={false}>
        <View style={styles.header}>
          <Text style={styles.logo}>Olá, Contador</Text>                                                                  <Text style={styles.subtitle}>Escritório Cuiabá Central</Text>
        </View>

        {/* Gráfico de Receitas */}
        <View style={styles.section}>
          <Text style={styles.sectionTitle}>Evolução de Receitas</Text>                                                   <LineChart
            data={{
              labels: ["Jan", "Fev", "Mar", "Abr", "Mai"],
              datasets: [{ data: [12, 19, 15, 22, 28] }]
            }}
            width={screenWidth - 40}
            height={180}                                            chartConfig={chartConfig}
            bezier
            style={{ borderRadius: 16 }}                          />
        </View>                                         
        {/* Módulos */}
        <View style={styles.section}>
          <Text style={styles.sectionTitle}>Módulos</Text>
          <View style={styles.modulesGrid}>                         <TouchableOpacity style={styles.moduleCard} onPress={() => navigation.navigate('Scanner')}>
              <Text style={styles.moduleText}>📸 Scanner</Text>
            </TouchableOpacity>
            <TouchableOpacity style={styles.moduleCard} onPress={() => navigation.navigate('Financeiro')}>                    <Text style={styles.moduleText}>💰 Financeiro</Text>
            </TouchableOpacity>
          </View>
        </View>
      </ScrollView>
    </SafeAreaView>
  );
}
                                                        // --- TELA DE SCANNER (CÂMERA) ---
function ScannerScreen() {
  const [image, setImage] = useState(null);

  const pickImage = async () => {
    let result = await ImagePicker.launchCameraAsync({ allowsEditing: true, quality: 0.5 });                        if (!result.canceled) setImage(result.assets[0].uri);
  };

  return (
    <View style={styles.containerCenter}>
      <Text style={styles.sectionTitle}>Escanear Nota Fiscal</Text>                                                   <TouchableOpacity style={styles.mainButton} onPress={pickImage}>                                                  <Text style={styles.buttonText}>Abrir Câmera</Text>
      </TouchableOpacity>
      {image && <Image source={{ uri: image }} style={styles.preview} />}
    </View>
  );
}                                                       
// --- NAVEGADOR ---
export default function App() {
  return (
    <NavigationContainer>
      <Stack.Navigator screenOptions={{ headerShown: false }}>
        <Stack.Screen name="Login" component={LoginScreen} />
        <Stack.Screen name="Home" component={HomeScreen} />
        <Stack.Screen name="Scanner" component={ScannerScreen} />
      </Stack.Navigator>
    </NavigationContainer>
  );
}                                                       
// --- ESTILOS E CONFIGS ---
const chartConfig = {
  backgroundColor: "#fff",
  backgroundGradientFrom: "#fff",
  backgroundGradientTo: "#fff",
  color: (opacity = 1) => `rgba(29, 78, 216, ${opacity})`,
  labelColor: (opacity = 1) => `rgba(100, 116, 139, ${opacity})`,
};
                                                        const styles = StyleSheet.create({
  container: { flex: 1, backgroundColor: '#f8fafc' },
  containerCenter: { flex: 1, justifyContent: 'center', alignItems: 'center', padding: 20 },
  loginContainer: { flex: 1, justifyContent: 'center', padding: 30, backgroundColor: '#fff' },
  loginLogo: { fontSize: 32, fontWeight: 'bold', textAlign: 'center', marginBottom: 40 },
  header: { backgroundColor: '#1d4ed8', padding: 30, borderBottomLeftRadius: 30, borderBottomRightRadius: 30 },
  logo: { color: '#fff', fontSize: 24, fontWeight: 'bold' },
  subtitle: { color: '#dbeafe' },
  section: { padding: 20 },
  sectionTitle: { fontSize: 18, fontWeight: 'bold', marginBottom: 15, color: '#1e293b' },
  input: { backgroundColor: '#f1f5f9', padding: 15, borderRadius: 12, marginBottom: 15, borderWidth: 1, borderColor: '#e2e8f0' },                                         mainButton: { backgroundColor: '#1d4ed8', padding: 18, borderRadius: 12, alignItems: 'center' },
  buttonText: { color: '#fff', fontWeight: 'bold' },
  modulesGrid: { flexDirection: 'row', justifyContent: 'space-between' },                                         moduleCard: { backgroundColor: '#fff', width: '48%', padding: 20, borderRadius: 20, elevation: 3, alignItems: 'center' },
  moduleText: { fontWeight: 'bold', color: '#1d4ed8' },
  preview: { width: 250, height: 350, marginTop: 20, borderRadius: 10 }
});
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:                                                    pkg install imagemagick
The program import is not installed. Install it by executing:                                                    pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
No command View, found, did you mean:
 Command view in package neovim-nightly,neovim
 Command view in package vim
 Command view in package vim-gtk from the x11-repo repository
SafeAreaView,: command not found
bash: syntax error near unexpected token `}'
The program import is not installed. Install it by executing:
 pkg install imagemagick
The program import is not installed. Install it by executing:
 pkg install imagemagick
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('            bash: //: Is a directory
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `{'            bash: syntax error near unexpected token `'Home''
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `'Erro','
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `<'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `}'
bash: //: Is a directory
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: {/*: No such file or directory
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: LineChart: No such file or directory              No command labels: found, did you mean:
 Command abcls in package alembic
 Command mlabel in package mtools
datasets:: command not found
No command }} found, did you mean:
 Command ab in package apache2
 Command at in package at                                Command bc in package bc
 Command ar in package binutils
 Command as in package binutils-bin
 Command ar in package binutils-is-llvm
 Command bk in package bk
 Command nc in package busybox
 Command cc in package clang
 Command [ in package coreutils
 Command lp in package cups
 Command d8 in package d8
 Command sh in package dash
 Command dx in package dx                                Command ed in package ed
 Command ef in package electric-fence
 Command et in package et
 Command fd in package fd
 Command fm in package fm
 Command fx in package fx
 Command dl in package gatling
 Command gh in package gh
 Command gs in package ghostscript
 Command gn in package gn
 Command go in package golang
 Command gm in package graphicsmagick
 Command gc in package graphviz
 Command gw in package gw from the x11-repo repository
 Command hx in package helix
 Command hh in package hstr
 Command hz in package hz
 Command i3 in package i3 from the x11-repo repository
 Command ip in package iproute2
 Command iw in package iw from the root-repo repository
 Command jo in package jo
 Command jq in package jq
 Command k in package kona
 Command lf in package lf                                Command pl in package libgnustep-base
 Command h3 in package libuber-h3                        Command lr in package lr
 Command lx in package lux-cli                           Command m4 in package m4
 Command mc in package mc
 Command ml in package mercury
 Command mg in package mg
 Command al in package mono
 Command ts in package moreutils
 Command lz in package mtools
 Command mu in package mu
 Command mr in package myrepos
 Command sc in package n-t-roff-sc
 Command ne in package ne
 Command ex in package neovim-nightly,neovim
 Command nc in package netcat-openbsd
 Command nc in package nmap
 Command pp in package nss-utils
 Command nu in package nushell
 Command nx in package nxengine from the x11-repo repository                                                     Command ol in package ol
 Command iv in package openimageio from the x11-repo repository
 Command o in package orbiton
 Command 7z in package p7zip
 Command gp in package pari
 Command pb in package pb
 Command ps in package procps
 Command pd in package proot-distro
 Command pv in package pv
 Command q in package q-dns-client
 Command r2 in package radare2
 Command rc in package rc
 Command ci in package rcs
 Command rg in package ripgrep
 Command rq in package rq
 Command ri in package ruby-ri
 Command sv in package runit
 Command rw in package rw
 Command sd in package sd
 Command ag in package silversearcher-ag
 Command sl in package sl
 Command st in package st from the x11-repo repository
 Command sr in package surfraw
 Command pt in package tcllib
 Command am in package termux-am
 Command df in package termux-tools
 Command ht in package texlive-bin
 Command sn in package tin-summer
 Command tf in package tinyfugue
 Command ug in package ugrep
 Command up in package up
 Command ul in package util-linux
 Command cu in package uucp
 Command uv in package uv
 Command ex in package vim
 Command ex in package vim-gtk from the x11-repo repository
 Command vt in package virustotal-cli
 Command vi in package vis
 Command wg in package wireguard-tools
 Command xh in package xh
 Command X in package xorg-server from the x11-repo repository
 Command xz in package xz-utils
 Command ya in package yazi
 Command yq in package yq
 Command z3 in package z3
 Command zk in package zk
No command - found, did you mean:
 Command [ in package coreutils
 Command k in package kona
 Command o in package orbiton
 Command q in package q-dns-client
 Command X in package xorg-server from the x11-repo repository
The program bezier is not installed. Install it by executing:
 pkg install mesa-demos, after running pkg install x11-repo
borderRadius:: command not found
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: {/*: No such file or directory
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'      bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `}'            bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: !result.canceled: event not found
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
No command {image found, did you mean:
 Command jimage in package openjdk-21
 Command jimage in package openjdk-25
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `}'
bash: //: Is a directory
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `)'
bash: syntax error near unexpected token `}'
bash: //: Is a directory
No command const found, did you mean:
 Command cpnt in package chntpw
 Command ctest in package cmake
 Command host in package dnsutils                        Command dunst in package dunst from the x11-repo repository
 Command gost in package gost
 Command count in package llvm-tools
 Command most in package most
 Command chpst in package runit                         backgroundColor:: command not found
backgroundGradientFrom:: command not found
backgroundGradientTo:: command not found
bash: syntax error near unexpected token `opacity'
bash: syntax error near unexpected token `opacity'
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `('
No command container: found, did you mean:
 Command containerd in package containerd from the root-repo repository
containerCenter:: command not found
loginContainer:: command not found
loginLogo:: command not found
No command header: found, did you mean:
 Command readelf in package binutils
 Command readelf in package binutils-is-llvm
 Command head in package coreutils
 Command heimer in package heimer from the x11-repo repository
 Command hexer in package hexer
No command logo: found, did you mean:
 Command lego in package lego
 Command login in package termux-tools
 Command look in package util-linux
subtitle:: command not found
No command section: found, did you mean:
 Command seticons in package wmaker from the x11-repo repository
sectionTitle:: command not found
No command input: found, did you mean:
 Command iauth in package ircd-irc2
 Command tput in package ncurses-utils
 Command npush in package npush
mainButton:: command not found
buttonText:: command not found
modulesGrid:: command not found
moduleCard:: command not found
moduleText:: command not found
No command preview: found, did you mean:
 Command permview in package mono
 Command rview in package vim
 Command eview in package vim-gtk from the x11-repo repository
bash: syntax error near unexpected token `}'
~ $ });
~ $ });
