# vim: ts=8:sw=8:noet
#
# Copyright (C) 2013 Red Hat, Inc.
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; version 2 of the License.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program; if not, write to the Free Software
# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
# MA  02110-1301, USA.  A copy of the GNU General Public License is
# also available at http://www.gnu.org/copyleft/gpl.html.

dist_bin_SCRIPTS = \
		   discover-host.rb \
		   find-missing-libs

if HAVE_SYSTEMD
dist_systemdsystemunit_DATA = discover-host.service
else
EXTRA_DIST = discover-host
initddir = $(sysconfdir)/rc.d/init.d
initd_SCRIPTS = discover-host
endif

dist_pkgdata_DATA = discovery-version-fact.rb

CLEANFILES = \
	     discover-host.rb \
	     discovery-version-fact.rb
